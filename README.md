# batter-incomplete


  # **********************************************************************************************
    # You found the bug. Great job!
    # **********************************************************************************************
    # todo: fix the bug by making sure the text value is set to the appropriate variable.
    def _draw_label(self, cast, group, format_str, data):
        label = cast.get_first_actor(group)
        text = label.get_text()
        text.set_value(format_str.format(data))
        position = label.get_position()
        self._video_service.draw_text(text, position)
