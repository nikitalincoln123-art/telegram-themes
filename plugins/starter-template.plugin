__id__ = "accent_color_changer"
__name__ = "Accent Color Changer"
__description__ = "Пример плагина для ExtraGram/AyuGram: меняет акцентный цвет интерфейса прямо из настроек. Стартовый шаблон для начинающих."
__author__ = "TGThemes"
__version__ = "1.0.0"
__icon__ = "emoji/1f3a8"
__app_version__ = ">=12.5.1"
__sdk_version__ = ">=1.4.0"

from base_plugin import BasePlugin
from java import jclass
from org.telegram.ui.ActionBar import Theme


class AccentColorChanger(BasePlugin):
    """Меняет акцентный цвет интерфейса на заданный.

    Это минимальный рабочий пример. Дополнительные методы:

    - ``on_load()``         — вызывается при загрузке / вкл. плагина
    - ``on_unload()``       — при выключении или удалении плагина
    - ``on_message(data)``  — хуки на сообщения
    """

    # Цвет в формате 0xAARRGGBB. Замените на свой.
    ACCENT_COLOR = 0xFF40D9C0

    def on_load(self):
        # Применяем акцент ко всем экранам клиента
        Theme.changeColor("<color name>", self.ACCENT_COLOR)
        # Обновляем темы после изменения цвета
        Theme.refreshTheme()

    def on_unload(self):
        # Возвращаем стандартный акцент клиента (бирюза)
        Theme.changeColor("<color name>", 0xFF3A76F0)
        Theme.refreshTheme()