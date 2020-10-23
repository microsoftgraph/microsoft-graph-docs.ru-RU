---
title: Тип ресурса Макоспривациакцессконтролитем
description: Представляет параметры конфиденциальности для отдельных процессов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63cd3a159562c9757267ca80203c256f8cc9b643
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701447"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>Тип ресурса Макоспривациакцессконтролитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет параметры конфиденциальности для отдельных процессов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя приложения, процесса или исполняемого файла.|
|идентификатор|Строка|Идентификатор пакета или путь к приложению, процессу или исполняемому файлу.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Идентификатор пакета используется для идентификации приложения. Путь используется для идентификации процесса или исполняемого файла. Возможные значения: `bundleID`, `path`.|
|кодерекуиремент|Строка|Введите требование к коду, которое можно получить с помощью команды "коконструирование – отобразить-r –" в приложении терминала. Включите все после "=>".|
|статиккодевалидатион|Логический|Статически проверяет требования к коду. Используйте этот параметр, если процесс делает недействительным свою подпись динамического кода.|
|блокккамера|Логический|Блокировка доступа к приложению "Камера".|
|блоккмикрофоне|Логический|Заблокируйте доступ к микрофону.|
|blockScreenCapture|Логический|Блокировать приложение от захвата содержимого отображения системы. Требуется macOS 10,15 или более поздняя версия.|
|блокклистеневент|Логический|Запретить приложению или процессу прослушивать события от устройств ввода, таких как мышь, клавиатура и траккпад. Требуется macOS 10,15 или более поздняя версия.|
|спичрекогнитион|[Включение](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к средству распознавания речи системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|вспомогатель|[Включение](../resources/intune-shared-enablement.md)|Разрешить приложению или процессу управлять MAC-адресом с помощью подсистемы специальных возможностей. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|addressBook|[Включение](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к контактным данным, управляемым контактами. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|calendar|[Включение](../resources/intune-shared-enablement.md)|Разрешите или блокируйте доступ к сведениям о событиях, которыми управляет календарь. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|напоминания|[Включение](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к информации, которая управляется напоминаниями. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|photos|[Включение](../resources/intune-shared-enablement.md)|Разрешите или блокируйте доступ к изображениям, управляемым фотографиями. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|медиалибрари|[Включение](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к музыке и библиотеке мультимедиа. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|филепровидерпресенце|[Включение](../resources/intune-shared-enablement.md)|Разрешите приложению или процессу доступ к файлам, управляемым расширением поставщика файлов другого приложения. Требуется macOS 10,15 или более поздняя версия. . Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполициаллфилес|[Включение](../resources/intune-shared-enablement.md)|Управление доступом ко всем защищенным файлам на устройстве. Файлы могут находиться в таких расположениях, как электронная почта, сообщения, приложения и административные параметры. Этот параметр следует применять с осторожностью. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполицисистемадминфилес|[Включение](../resources/intune-shared-enablement.md)|Разрешить приложению или процессу доступ к файлам, используемым в системном администрировании. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполицидесктопфолдер|[Включение](../resources/intune-shared-enablement.md)|Разрешите или заблокируйте доступ к папке "Рабочий стол". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполицидокументсфолдер|[Включение](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к папке "документы". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполицидовнлоадсфолдер|[Включение](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к папке "загрузки". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполицинетворкволумес|[Включение](../resources/intune-shared-enablement.md)|Разрешите или заблокируйте доступ к сетевым томам. Требуется macOS 10,15 или более поздняя версия. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|системполициремоваблеволумес|[Включение](../resources/intune-shared-enablement.md)|Управление доступом к съемным томам на устройстве, например внешнему жесткому диску. Требуется macOS 10,15 или более поздняя версия. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Четный|[Включение](../resources/intune-shared-enablement.md)|Управление доступом к API Кореграфикс, которые используются для отправки Кжевентс в поток системных событий. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|аппливентсалловедрецеиверс|Коллекция [макосаппливентрецеивер](../resources/intune-deviceconfig-macosappleeventreceiver.md)|Разрешить или запретить приложению или процессу отправку ограниченного события Apple другому приложению или процессу. Необходимо знать идентификатор, тип идентификатора и требования к коду принимающего приложения или процесса. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSPrivacyAccessControlItem",
  "displayName": "String",
  "identifier": "String",
  "identifierType": "String",
  "codeRequirement": "String",
  "staticCodeValidation": true,
  "blockCamera": true,
  "blockMicrophone": true,
  "blockScreenCapture": true,
  "blockListenEvent": true,
  "speechRecognition": "String",
  "accessibility": "String",
  "addressBook": "String",
  "calendar": "String",
  "reminders": "String",
  "photos": "String",
  "mediaLibrary": "String",
  "fileProviderPresence": "String",
  "systemPolicyAllFiles": "String",
  "systemPolicySystemAdminFiles": "String",
  "systemPolicyDesktopFolder": "String",
  "systemPolicyDocumentsFolder": "String",
  "systemPolicyDownloadsFolder": "String",
  "systemPolicyNetworkVolumes": "String",
  "systemPolicyRemovableVolumes": "String",
  "postEvent": "String",
  "appleEventsAllowedReceivers": [
    {
      "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
      "codeRequirement": "String",
      "identifier": "String",
      "identifierType": "String",
      "allowed": true
    }
  ]
}
```





