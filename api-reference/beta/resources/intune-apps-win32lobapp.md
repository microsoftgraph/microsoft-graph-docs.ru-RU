---
title: Тип ресурса win32LobApp
description: Содержит свойства и наследуемые свойства для приложений Win32.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6cd1a0d715ba4c9ebcd26d88edcefcd0136bf919
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842772"
---
# <a name="win32lobapp-resource-type"></a>Тип ресурса win32LobApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства и наследуемые свойства для приложений Win32.

Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список win32LobApps](../api/intune-apps-win32lobapp-list.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md) коллекции|Свойства списка и связей объектов [win32LobApp](../resources/intune-apps-win32lobapp.md) .|
|[Получение win32LobApp](../api/intune-apps-win32lobapp-get.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Чтение свойства и связи объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .|
|[Создание win32LobApp](../api/intune-apps-win32lobapp-create.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Создание нового объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .|
|[Удаление win32LobApp](../api/intune-apps-win32lobapp-delete.md)|Нет|Удаляет [win32LobApp](../resources/intune-apps-win32lobapp.md).|
|[Обновление win32LobApp](../api/intune-apps-win32lobapp-update.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Обновление свойства объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|описание|String|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Большой значок, который отображается в сведениях о приложении и используется для отправки значка. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Примечания к приложению. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Состояние передачи. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|installCommandLine|Строка|Командной строки для установки этого приложения|
|uninstallCommandLine|Строка|В командной строке команду Удалить это приложение|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Архитектура Windows, которая поддерживается этим приложением. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Значение, указывающее минимальную применимую версию операционной системы.|
|minimumFreeDiskSpaceInMB|Int32|Значение для минимального свободного дискового пространства, которая требуется для установки этого приложения.|
|minimumMemoryInMB|Int32|Значение для минимального физической памяти, которая требуется для установки этого приложения.|
|minimumNumberOfProcessors|Int32|Значение для минимальное число процессоров которая требуется для установки этого приложения.|
|minimumCpuSpeedInMHz|Int32|Значение для минимальная скорость ЦП, которая требуется для установки этого приложения.|
|detectionRules|[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) коллекции|Определение правил для обнаружения Win32 строки из бизнес-приложения.|
|installExperience|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|Опыт установки для этого приложения.|
|returnCodes|[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) коллекции|Коды возврата для записи поведение при установке.|
|msiInformation|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|Подробности MSI, если это приложение Win32 представляет собой приложение MSI.|
|setupFilePath|Строка|Относительный путь к файлу программы установки в пакете зашифрованные Win32LobApp.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Сводка по установке мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) коллекции|Список состояния установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) коллекции|Список состояния установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Коллекция объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

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
    "v10_1803": true
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
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "String"
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
    "packageType": "String"
  },
  "setupFilePath": "String"
}
```





