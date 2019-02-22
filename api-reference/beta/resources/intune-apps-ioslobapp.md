---
title: Тип ресурса iosLobApp
description: Содержит свойства, в том числе унаследованные, для бизнес-приложений iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d08dc7901c4dbd7f1d384d45b49fa40e5ce6767
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152803"
---
# <a name="ioslobapp-resource-type"></a>Тип ресурса iosLobApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, в том числе унаследованные, для бизнес-приложений iOS.


Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosLobApps](../api/intune-apps-ioslobapp-list.md)|Коллекция [iosLobApp](../resources/intune-apps-ioslobapp.md)|Список свойств и связей объектов [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Получение iosLobApp](../api/intune-apps-ioslobapp-get.md)|[iosLobApp](../resources/intune-apps-ioslobapp.md);|Считывание свойств и связей объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Создание iosLobApp](../api/intune-apps-ioslobapp-create.md)|[iosLobApp](../resources/intune-apps-ioslobapp.md);|Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Удаление iosLobApp](../api/intune-apps-ioslobapp-delete.md)|None|Удаление экземпляра [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Обновление iosLobApp](../api/intune-apps-ioslobapp-update.md)|[iosLobApp](../resources/intune-apps-ioslobapp.md)|Обновление свойств объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
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
|uploadState|Int32|Состояние отправки. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[Мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Логический|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|bundleId|String|Имя удостоверения.|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|Архитектура iOS, поддерживаемая этим приложением.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosminimumoperatingsystem.md)|Значение, указывающее минимальную применимую версию операционной системы.|
|expirationDateTime|DateTimeOffset|Время окончания срока действия.|
|versionNumber|String|Номер версии бизнес-приложения для iOS.|
|buildNumber|String|Номер сборки бизнес-приложения для iOS.|
|identityVersion|String|Версия удостоверения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Сводка по установке мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Коллекция объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String",
  "identityVersion": "String"
}
```




