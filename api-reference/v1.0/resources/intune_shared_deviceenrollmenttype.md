# <a name="deviceenrollmenttype-enum-type"></a>тип перечисления deviceEnrollmentType

> **Важно:** API бета-версии в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные способы добавления мобильного устройства для управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|неизвестный|0|Значение по умолчанию, тип регистрации не собираются.|
|userEnrollment|1|Регистрация управляемаяпользователем по каналу BYOD.|
|deviceEnrollmentManager|2|Регистрация пользователя с учетной записью диспетчера устройства.|
|appleBulkWithUser|3|Массовое включение Apple с вызовом пользователя (DEP, Apple Configurator).|
|appleBulkWithoutUser|4|Массовое включение Apple без вызова пользователя (DEP, Apple Configurator, Mobile Config).|
|windowsAzureADJoin|5|Windows 10 Azure AD Join.|
|windowsBulkUserless|6|Массовая регистрация Windows 10 через ICD с сертификатом.|
|windowsAutoEnrollment|7|Windows 10 автоматическая регистрация. (Добавление рабочей учетной записи)|
|windowsBulkAzureDomainJoin|8|Windows 10 bulk Azure AD Join.|
|windowsCoManagement|9|Совместное управление Windows 10, инициированное AutoPilot или групповой политикой.|



