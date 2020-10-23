---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6d880971d86029d1a18001b2eafd6459d15d156
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731368"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a>Создание androidDeviceOwnerGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.

В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|аккаунтсблоккмодификатион|Логический|Указывает, отключено ли добавление или удаление учетных записей.|
|аппсалловинсталлфромункновнсаурцес|Логический|Указывает, может ли пользователь включить параметр "неизвестные источники".|
|аппсаутаупдатеполици|[андроиддевицеовнераппаутаупдатеполицитипе](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|аппсдефаултпермиссионполици|[андроиддевицеовнердефаултапппермиссионполицитипе](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|аппсрекоммендскиппингфирстусехинтс|Логический|Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.|
|блуетусблоккконфигуратион|Логический|Указывает, следует ли запретить пользователю настраивать Bluetooth.|
|блуетусблоккконтактшаринг|Логический|Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.|
|cameraBlocked|Boolean|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|цертификатекредентиалконфигуратиондисаблед|Логический|Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.|
|микрософтлаунчерконфигуратионенаблед|Логический|Указывает, следует ли настроить средство запуска Microsoft.|
|микрософтлаунчеркустомваллпаперенаблед|Логический|Указывает, следует ли настраивать фоновый рисунок на целевых устройствах.|
|микрософтлаунчеркустомваллпаперимажеурл|Строка|Указывает URL-адрес для файла изображения, который будет использоваться в качестве фонового рисунка на целевых устройствах.|
|микрософтлаунчеркустомваллпапералловусермодификатион|Логический|Указывает, может ли пользователь изменять фоновый рисунок для персонализации своего устройства.|
|микрософтлаунчерфиденаблед|Логический|Указывает, следует ли включить веб-канал запуска на устройстве.|
|микрософтлаунчерфидалловусермодификатион|Логический|Указывает, может ли пользователь изменять веб-канал запуска на устройстве.|
|микрософтлаунчердоккпресенцеконфигуратион|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Указывает, следует ли настроить закрепление устройства. Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.|
|микрософтлаунчердоккпресенцеалловусермодификатион|Логический|Указывает, может ли пользователь изменять конфигурацию закрепления устройств на устройстве.|
|микрософтлаунчерсеарчбарплацементконфигуратион|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Указывает конфигурацию размещения панели поиска на устройстве. Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Указывает, какой профиль регистрации вы хотите настроить. Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|датароамингблоккед|Логический|Указывает, следует ли запретить пользователю перемещать данные.|
|датетимеконфигуратионблоккед|Логический|Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.|
|факториресетдевицеадминистраторемаилс|Коллекция строк|Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр Reset фабрики в параметрах.|
|глобалпрокси|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.|
|гуглеаккаунтсблоккед|Логический|Указывает, будут ли блокироваться учетные записи Google.|
|киоскмодескринсаверконфигуратионенаблед|Логический|Указывает, следует ли включить режим экранной заставки или не в режиме киоска.|
|киоскмодескринсаверимажеурл|Строка|URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.|
|киоскмодескринсавердисплайтимеинсекондс|Int32|Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска. Допустимые значения — от 0 до 9999999|
|киоскмодескринсаверстартделайинсекондс|Int32|Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска. Допустимые значения — от 1 до 9999999|
|киоскмодескринсавердетектмедиадисаблед|Логический|Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|киоскмодеваллпаперурл|Строка|URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.|
|киоскмодикситкоде|Строка|Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.|
|киоскмодевиртуалхомебуттоненаблед|Логический|Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.|
|киоскмодевиртуалхомебуттонтипе|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой". Возможные значения: `notConfigured`, `swipeUp`, `floating`.|
|киоскмодеблуетусконфигуратионенаблед|Логический|Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.|
|киоскмодевификонфигуратионенаблед|Логический|Указывает, следует ли запретить пользователю настраивать параметры Wi-Fi в режиме киоска.|
|киоскмодефлашлигхтконфигуратионенаблед|Логический|Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.|
|киоскмодемедиаволумеконфигуратионенаблед|Логический|Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.|
|киоскмодешовдевицеинфо|Логический|Указывает, следует ли разрешить пользователю доступ к сведениям о базовом устройстве.|
|киоскмодеманажедсеттингсентридисаблед|Логический|Указывает, следует ли отображать точку входа управляемых параметров на управляемом домашнем экране в режиме киоска.|
|киоскмодедебугменуеасякцессенаблед|Логический|Указывает, следует ли запретить пользователю простой доступ к меню Отладка в режиме киоска.|
|киоскмодешоваппнотификатионбадже|Логический|Указывает, следует ли отображать эмблемы уведомлений приложений в режиме киоска.|
|киоскмодескринориентатион|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Конфигурация ориентации экрана для управляемого экрана дома в режиме киоска. Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|киоскмодеиконсизе|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Конфигурация размера значков для управляемого экрана дома в режиме киоска. Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|киоскмодефолдерикон|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Конфигурация значков папок для управляемого экрана дома в режиме киоска. Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|киоскмодевифиалловедссидс|Коллекция строк|Ограниченный набор подключений WIFI SSID, доступных пользователю для настройки в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|микрофонефорцемуте|Логический|Указывает, следует ли запретить разблокирование микрофона устройства.|
|нетворкескапехатчалловед|Логический|Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.|
|нфкблоккаутгоингбеам|Логический|Указывает, следует ли заблокировать исходящую форму NFC.|
|пассвордблокккэйгуард|Логический|Указывает, отключен ли кэйгуард.|
|пассвордблокккэйгуардфеатурес|Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список компонентов кэйгуард устройств, которые необходимо заблокировать. Эта коллекция может содержать не более 7 элементов. Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.|
|passwordExpirationDays|Int32|Указывает период времени, в течение которого можно задать пароль до истечения срока его действия, а также потребуется новый пароль. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Указывает минимальную длину пароля, необходимого для устройства. Допустимые значения: от 4 до 16.|
|пассвордминимумлеттерчарактерс|Int32|Указывает минимальное число символов, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумловеркасечарактерс|Int32|Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумнонлеттерчарактерс|Int32|Указывает минимальное количество небуквенных символов, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумнумерикчарактерс|Int32|Указывает минимальное количество числовых символов, необходимое для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумсимболчарактерс|Int32|Указывает минимальное число символов, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумупперкасечарактерс|Int32|Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|пассвордпревиауспассвордкаунттоблокк|Int32|Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале. Допустимые значения: от 0 до 24.|
|passwordRequiredType|[андроиддевицеовнеррекуиредпассвордтипе](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое для устройства. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства. Допустимые значения: от 4 до 11.|
|плайсторемоде|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Указывает режим проигрывания устройства в хранилище. Возможные значения: `notConfigured`, `allowList`, `blockList`.|
|сафебутблоккед|Логический|Указывает, отключена ли загрузка устройства в "безопасная загрузка".|
|screenCaptureBlocked|Boolean|Указывает, следует ли отключить возможность использования снимков экрана.|
|секуритялловдебуггингфеатурес|Логический|Указывает, следует ли запретить пользователю включать функции отладки на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуется ли проверка приложений.|
|статусбарблоккед|Логический|Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.|
|стайонмодес|Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых дисплей устройства остается включенным. Эта коллекция может содержать не более 4 элементов. Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.|
|сторажеалловусб|Логический|Указывает, следует ли разрешить запоминающее устройство USB.|
|сторажеблоккекстерналмедиа|Логический|Указывает, следует ли заблокировать внешний носитель.|
|сторажеблоккусбфилетрансфер|Логический|Указывает, следует ли запретить передачу файлов через USB.|
|системупдатевиндовстартминутесафтермиднигхт|Int32|Указывает количество минут после полуночи, когда запустится окно обновления системы. Допустимые значения — от 0 до 1440|
|системупдатевиндовендминутесафтермиднигхт|Int32|Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы. Допустимые значения — от 0 до 1440|
|системупдатеинсталлтипе|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|системвиндовсблоккед|Логический|Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.|
|усерсблоккадд|Логический|Указывает, отключено ли добавление пользователей и профилей.|
|усерсблоккремове|Логический|Указывает, следует ли отключить удаление других пользователей с устройства.|
|волумеблоккаджустмент|Логический|Указывает, отключена ли настройка главного тома.|
|впналвайсонлоккдовнмоде|Логический|Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.|
|Свойства vpnalwaysonpackageidentifier|Строка|Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.|
|вифиблоккедитконфигуратионс|Логический|Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.|
|вифиблоккедитполицидефинедконфигуратионс|Логический|Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.|
|персоналпрофилеаппсалловинсталлфромункновнсаурцес|Логический|Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.|
|персоналпрофилекамераблоккед|Логический|Указывает, следует ли отключить использование камеры в личном профиле.|
|персоналпрофилескринкаптуреблоккед|Логический|Указывает, следует ли отключить возможность делать снимки экрана в личном профиле.|
|workProfilePasswordExpirationDays|Int32|Указывает количество дней, в течение которых может быть установлен пароль рабочего профиля до истечения срока действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Указывает минимальную длину пароля рабочего профиля. Допустимые значения: от 4 до 16.|
|воркпрофилепассвордминимумнумерикчарактерс|Int32|Указывает минимальное количество числовых символов, необходимое для пароля рабочего профиля. Допустимые значения — от 1 до 16.|
|воркпрофилепассвордминимумнонлеттерчарактерс|Int32|Указывает минимальное количество небуквенных символов, необходимых для пароля рабочего профиля. Допустимые значения — от 1 до 16.|
|воркпрофилепассвордминимумлеттерчарактерс|Int32|Указывает минимальное число символов, необходимых для пароля рабочего профиля. Допустимые значения — от 1 до 16.|
|воркпрофилепассвордминимумловеркасечарактерс|Int32|Указывает минимальное количество символов нижнего регистра, необходимых для пароля рабочего профиля. Допустимые значения — от 1 до 16.|
|воркпрофилепассвордминимумупперкасечарактерс|Int32|Указывает минимальное количество символов в верхнем регистре, необходимое для пароля рабочего профиля. Допустимые значения — от 1 до 16.|
|воркпрофилепассвордминимумсимболчарактерс|Int32|Указывает минимальное число символов, необходимых для пароля рабочего профиля. Допустимые значения — от 1 до 16.|
|воркпрофилепассвордпревиауспассвордкаунттоблокк|Int32|Указывает длину журнала паролей рабочего профиля, в котором пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале. Допустимые значения: от 0 до 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз пользователь может ввести неправильный пароль рабочего профиля, прежде чем устройство будет очищено. Допустимые значения: от 4 до 11.|
|workProfilePasswordRequiredType|[андроиддевицеовнеррекуиредпассвордтипе](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое для пароля рабочего профиля. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 6096

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 6268

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```





