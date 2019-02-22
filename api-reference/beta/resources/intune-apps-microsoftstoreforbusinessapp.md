---
title: Тип ресурса microsoftStoreForBusinessApp
description: Приложения из Microsoft Store для бизнеса. Этот класс не поддерживает операции создания, удаления и обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9e3af80268483b8665dbcc62c0579dc8b5fbca3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169876"
---
# <a name="microsoftstoreforbusinessapp-resource-type"></a>Тип ресурса microsoftStoreForBusinessApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Приложения из Microsoft Store для бизнеса. Этот класс не поддерживает операции создания, удаления и обновления.


Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление microsoftStoreForBusinessApps](../api/intune-apps-microsoftstoreforbusinessapp-list.md)|Коллекция [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|Список свойств и связей объектов [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Получение microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-get.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md);|Считывание свойств и связей объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Создание microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-create.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md);|Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Удаление microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-delete.md)|None|Удаление экземпляра [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Обновление microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-update.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|

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
|usedLicenseCount|Int32|Количество используемых лицензий Microsoft Store для бизнеса.|
|totalLicenseCount|Int32|Общее количество лицензий Microsoft Store для бизнеса.|
|productKey|Строка|Ключ продукта для приложения.|
|licenseType|[Микрософтсторефорбусинесслиценсетипе](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|Тип лицензии приложения. Возможные значения: `offline`, `online`.|
|packageIdentityName|String|Идентификатор пакета приложения.|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|Поддерживаемый тип лицензии.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Сводка по установке мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|containedApps|Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|Коллекция вложенных приложений в mobileApp, действующая в виде пакета.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




