---
title: тип ресурса windowsStoreApp
description: Содержит свойства и унаследованные свойства для приложений Windows Store.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1fe01d10c960d9844d382bc0024d1f186aefca93
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091855"
---
# <a name="windowsstoreapp-resource-type"></a>тип ресурса windowsStoreApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для приложений Windows Store.


Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsStoreApps](../api/intune-apps-windowsstoreapp-list.md)|[коллекция windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Список свойств и связей объектов [WindowsStoreApp.](../resources/intune-apps-windowsstoreapp.md)|
|[Получить WindowsStoreApp](../api/intune-apps-windowsstoreapp-get.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Чтение свойств и связей объекта [WindowsStoreApp.](../resources/intune-apps-windowsstoreapp.md)|
|[Создание WindowsStoreApp](../api/intune-apps-windowsstoreapp-create.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Создание нового [объекта WindowsStoreApp.](../resources/intune-apps-windowsstoreapp.md)|
|[Удаление WindowsStoreApp](../api/intune-apps-windowsstoreapp-delete.md)|Нет|Удаляет [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).|
|[Обновление WindowsStoreApp](../api/intune-apps-windowsstoreapp-update.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Обновление свойств объекта [WindowsStoreApp.](../resources/intune-apps-windowsstoreapp.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|description|String|Описание приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|uploadState|Int32|Состояние загрузки. Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` . Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению по крайней мере одна группа. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция объектов string|Список ids тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|dependentAppCount|Int32|Общее число зависимостей, которые имеет детское приложение. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersedingAppCount|Int32|Общее число приложений, которые это приложение прямо или косвенно перемежает. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersededAppCount|Int32|Общее число приложений, которые это приложение прямо или косвенно вымежает. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|appStoreUrl|String|URL Windows магазина приложений.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|deviceStatuses|[коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояния установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|userStatuses|[коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояния установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|отношения|[коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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
  "appStoreUrl": "String"
}
```



