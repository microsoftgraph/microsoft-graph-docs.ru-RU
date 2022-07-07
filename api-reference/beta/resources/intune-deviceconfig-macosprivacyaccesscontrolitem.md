---
title: Тип ресурса macOSPrivacyAccessControlItem
description: Представляет параметры конфиденциальности для каждого процесса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be98e81399edc9682797f1b1aa7f04d1f02803bf
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669072"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>Тип ресурса macOSPrivacyAccessControlItem

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет параметры конфиденциальности для каждого процесса.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя приложения, процесса или исполняемого файла.|
|идентификатор|String|Идентификатор пакета или путь приложения, процесса или исполняемого файла.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Идентификатор пакета используется для идентификации приложения. Путь используется для идентификации процесса или исполняемого файла. Возможные значения: `bundleID`, `path`.|
|codeRequirement|String|Введите требование к коду, которое можно получить с помощью команды "codesign -display -r -" в приложении терминала. Включите все после "=>".|
|staticCodeValidation|Boolean|Статически проверяет требования к коду. Используйте этот параметр, если процесс недействителен для своей динамической сигнатуры кода.|
|blockCamera|Логическое|Блокировать доступ к приложению камеры.|
|blockMicrophone|Логическое|Блокировать доступ к микрофону.|
|blockScreenCapture|Логическое|Запретить приложению захват содержимого системного дисплея. Требуется macOS 10.15 или более поздней версии.|
|blockListenEvent|Логическое|Запретить приложению или процессу прослушивать события с устройств ввода, таких как мышь, клавиатура и trackpad. Требуется macOS 10.15 или более поздней версии.|
|speechRecognition|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешите или заблокируют доступ к системному речевом распознаванию. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Доступность|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешите приложению или процессу управлять компьютером Mac с помощью подсистемы специальных возможностей. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|addressBook|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешите или заблокируете доступ к контактным данным, управляемым контактами. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|calendar|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешить или заблокировать доступ к сведениям о событиях, управляемых календарем. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Напоминания|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешите или заблокируете доступ к информации, управляемой напоминаниями. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|photos|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешение или блокировка доступа к изображениям, управляемым службой "Фотографии". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|mediaLibrary|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешить или заблокировать доступ к музыке и библиотеке мультимедиа. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|fileProviderPresence|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешить приложению или процессу доступ к файлам, управляемым расширением поставщика файлов другого приложения. Требуется macOS 10.15 или более поздней версии. . Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyAllFiles|[Включения](../resources/intune-deviceconfig-enablement.md)|Управление доступом ко всем защищенным файлам на устройстве. Файлы могут быть в таких расположениях, как сообщения электронной почты, сообщения, приложения и параметры администрирования. Примените этот параметр с осторожностью. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicySystemAdminFiles|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешить приложению или процессу доступ к файлам, используемым при администрировании системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDesktopFolder|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешить или заблокировать доступ к папке "Рабочий стол". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDocumentsFolder|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешить или заблокировать доступ к папке "Документы". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDownloadsFolder|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешите или заблокируете доступ к папке "Загрузки". Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyNetworkVolumes|[Включения](../resources/intune-deviceconfig-enablement.md)|Разрешите или заблокируете доступ к сетевым томам. Требуется macOS 10.15 или более поздней версии. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyRemovableVolumes|[Включения](../resources/intune-deviceconfig-enablement.md)|Управление доступом к съемным томам на устройстве, например внешнему жесткому диску. Требуется macOS 10.15 или более поздней версии. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|postEvent|[Включения](../resources/intune-deviceconfig-enablement.md)|Управление доступом к API CoreGraphics, которые используются для отправки CGEvents в системный поток событий. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|appleEventsAllowedReceivers|[Коллекция macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md)|Разрешить или запретить приложению или процессу отправлять ограниченное событие Apple другому приложению или процессу. Необходимо знать идентификатор, тип идентификатора и требования к коду принимающего приложения или процесса. Эта коллекция может содержать не более 500 элементов.|

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




