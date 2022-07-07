---
title: Тип ресурса win32LobApp
description: Содержит свойства и унаследованные свойства для приложений Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c5c5d4edb0afd32a7bf9c5666a4a307b85ea8760
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669275"
---
# <a name="win32lobapp-resource-type"></a>Тип ресурса win32LobApp

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для приложений Win32.


Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление win32LobApps](../api/intune-apps-win32lobapp-list.md)|[Коллекция win32LobApp](../resources/intune-apps-win32lobapp.md)|Список свойств и связей объектов [win32LobApp](../resources/intune-apps-win32lobapp.md) .|
|[Получение win32LobApp](../api/intune-apps-win32lobapp-get.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Чтение свойств и связей объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .|
|[Создание win32LobApp](../api/intune-apps-win32lobapp-create.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Создайте новый [объект win32LobApp](../resources/intune-apps-win32lobapp.md) .|
|[Удаление win32LobApp](../api/intune-apps-win32lobapp-delete.md)|Нет|Удаляет [win32LobApp](../resources/intune-apps-win32lobapp.md).|
|[Обновление win32LobApp](../api/intune-apps-win32lobapp-update.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|String|Описание приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Состояние отправки. Возможные значения: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению хотя бы одна группа. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|dependentAppCount|Int32|Общее количество зависимостей, которые имеет дочернее приложение. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|supersedingAppCount|Int32|Общее количество приложений, которые это приложение прямо или косвенно заменяет. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|supersededAppCount|Int32|Общее количество приложений, на которые это приложение прямо или косвенно заменяется. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|installCommandLine|String|Командная строка для установки этого приложения|
|uninstallCommandLine|String|Командная строка для удаления этого приложения|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md);|Архитектура Windows, которая поддерживается этим приложением. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|
|minimumFreeDiskSpaceInMB|Int32|Значение минимального свободного места на диске, необходимого для установки этого приложения.|
|minimumMemoryInMB|Int32|Значение минимального объема физической памяти, необходимого для установки этого приложения.|
|minimumNumberOfProcessors|Int32|Значение минимального количества процессоров, необходимое для установки этого приложения.|
|minimumCpuSpeedInMHz|Int32|Значение минимальной скорости ЦП, необходимой для установки этого приложения.|
|detectionRules|[Коллекция win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)|Правила обнаружения для обнаружения приложения Win32 Line of Business (LoB).|
|requirementRules|[Коллекция win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|Правила требований для обнаружения приложения Win32 Line of Business (LoB).|
|правила|[Коллекция win32LobAppRule](../resources/intune-apps-win32lobapprule.md)|Правила обнаружения и требования для этого приложения.|
|installExperience|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|Интерфейс установки для этого приложения.|
|returnCodes|[Коллекция win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)|Коды возврата для поведения после установки.|
|msiInformation|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|Сведения о MSI, если это приложение Win32 является приложением MSI.|
|setupFilePath|String|Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.|
|minimumSupportedWindowsRelease|String|Значение минимального поддерживаемого выпуска Windows.|
|displayVersion|String|Версия, отображаемая в пользовательском интерфейсе для этого приложения.|
|allowAvailableUninstall|Логическое|Значение TRUE указывает, что удаление поддерживается с корпоративного портала для приложения Windows (Win32) с доступным назначением. Значение FALSE указывает, что удаление не поддерживается для приложения Windows (Win32) с доступным назначением. Значение по умолчанию — FALSE.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Отношения|[Коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32LobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "installCommandLine": "String",
  "uninstallCommandLine": "String",
  "applicableArchitectures": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true,
    "v10_2H20": true,
    "v10_21H1": true
  },
  "minimumFreeDiskSpaceInMB": 1024,
  "minimumMemoryInMB": 1024,
  "minimumNumberOfProcessors": 1024,
  "minimumCpuSpeedInMHz": 1024,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String",
      "operator": "String",
      "detectionValue": "String"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "String",
      "detectionValue": "String",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "String",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "operationType": "String",
      "operator": "String",
      "comparisonValue": "String"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "String",
    "deviceRestartBehavior": "String"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 1024,
      "type": "String"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "String",
    "productVersion": "String",
    "upgradeCode": "String",
    "requiresReboot": true,
    "packageType": "String",
    "productName": "String",
    "publisher": "String"
  },
  "setupFilePath": "String",
  "minimumSupportedWindowsRelease": "String",
  "displayVersion": "String",
  "allowAvailableUninstall": true
}
```




