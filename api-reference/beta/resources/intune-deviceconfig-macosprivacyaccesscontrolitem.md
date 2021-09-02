---
title: тип ресурса macOSPrivacyAccessControlItem
description: Представляет параметры конфиденциальности для каждого процесса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 158729518b47be682e00bea9d77b8a7308c9d4b1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789638"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>тип ресурса macOSPrivacyAccessControlItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет параметры конфиденциальности для каждого процесса.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени приложения, процесса или исполняемого.|
|идентификатор|Строка|ID пакета или путь приложения, процесса или исполняемого.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Для идентификации приложения используется идентификация пакета. Путь используется для определения процесса или выполнения. Возможные значения: `bundleID`, `path`.|
|codeRequirement|Строка|Введите требование кода, которое можно получить с командой "codeign -display-r-" в приложении Терминал. Включай все после '=>'.|
|staticCodeValidation|Логический|Статически проверяет требование кода. Используйте этот параметр, если процесс недействителен для динамической подписи кода.|
|blockCamera|Логический|Блокировка доступа к приложению камеры.|
|blockMicrophone|Логический|Блокировка доступа к микрофону.|
|blockScreenCapture|Логический|Блокировка приложения от захвата содержимого дисплея системы. Требуется macOS 10.15 или более поздней.|
|blockListenEvent|Boolean|Блокирование приложения или процесса прослушивания событий с устройств ввода, таких как мышь, клавиатура и трекпад. Требуется macOS 10.15 или более поздней.|
|speechRecognition|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к объекту распознавания речи системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|доступность|[включить](../resources/intune-shared-enablement.md)|Разрешить приложению или процессу управлять Mac с помощью подсистемы доступности. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|addressBook|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к контактной информации, управляемой контактами. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|calendar|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к сведениям о событиях, управляемых Calendar. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|напоминания|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к сведениям, управляемым reminders. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|photos|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к изображениям, управляемым Фото. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|mediaLibrary|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к музыке и медиатеке. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|fileProviderPresence|[включить](../resources/intune-shared-enablement.md)|Разрешить приложению или процессу доступ к файлам, управляемым расширением поставщика файлов другого приложения. Требуется macOS 10.15 или более поздней. . Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyAllFiles|[включить](../resources/intune-shared-enablement.md)|Управление доступом ко всем защищенным файлам на устройстве. Файлы могут быть в таких местах, как электронная почта, сообщения, приложения и параметры администрирования. Применяйте этот параметр с осторожностью. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicySystemAdminFiles|[включить](../resources/intune-shared-enablement.md)|Разрешить приложению или процессу доступ к файлам, используемым при администрировании системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDesktopFolder|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к папке Desktop. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDocumentsFolder|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к папке Documents. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDownloadsFolder|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к папке Downloads. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyNetworkVolumes|[включить](../resources/intune-shared-enablement.md)|Разрешить или заблокировать доступ к сетевым томам. Требуется macOS 10.15 или более поздней. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyRemovableVolumes|[включить](../resources/intune-shared-enablement.md)|Управление доступом к съемным томам на устройстве, например к внешнему жесткому диску. Требуется macOS 10.15 или более поздней. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|postEvent|[включить](../resources/intune-shared-enablement.md)|Управление доступом к API CoreGraphics, которые используются для отправки CGEvents в поток событий системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|appleEventsAllowedReceivers|[коллекция macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md)|Разрешить или запретить приложению или процессу отправлять ограниченное событие Apple в другое приложение или процесс. Необходимо знать идентификатор, тип идентификатора и требования к коду для получения приложения или процесса. Эта коллекция может содержать не более 500 элементов.|

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



