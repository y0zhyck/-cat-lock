# -cat-lock
1) Заблокируйте клавиатуру с помощью горячих клавиш (Ctrl + L). Вы увидите полупрозрачную накладку, указывающую на то, что клавиатура заблокирована, что обеспечивает непрерывный просмотр.
2) Разблокируйте клавиатуру, нажав на накладку.
3) Откройте параметры конфигурации через удобное меню в системном трее:
4) Отрегулируйте непрозрачность наложения в соответствии с вашими предпочтениями.
5) Включите или отключите системные уведомления, когда клавиатура заблокирована.

---

pip install pyinstaller

pyinstaller --onefile --add-data="./resources/img/icon.ico:./resources/img/" --add-data="./resources/img/icon.png:./resources/img/" --add-data="./resources/config/config.json:./resources/config/" --icon="./resources/img/icon.ico" --hidden-import plyer.platforms.win.notification --noconsole --name="CatLock" "./src/main.py"


Полагается на https://github.com/boppreh/keyboard /, который полностью поддерживает только Windows
Горячие клавиши, привязанные к операционной системе, имеют приоритет, например, ctrl + alt + del (таким образом, вы не будете заблокированы, если что-то пойдет не так).


Tested by:

![image](https://github.com/y0zhyck/-cat-lock/assets/38162408/09ebbfe6-efa9-4bb7-8949-171bae189aaf)
