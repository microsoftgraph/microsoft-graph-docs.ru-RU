---
title: Тип ресурса androidManagedStoreWebApp
description: Содержит свойства и унаследованные свойства для веб-приложений, настроенных для распределения через управляемый магазин приложений Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75729e972cd08b9c61d9992e7c46dfe2d99200e5
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669366"
---
# <a name="androidmanagedstorewebapp-resource-type"></a>Тип ресурса androidManagedStoreWebApp

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для веб-приложений, настроенных для распределения через управляемый магазин приложений Android.


Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление androidManagedStoreWebApps](../api/intune-apps-androidmanagedstorewebapp-list.md)|[Коллекция androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Список свойств и связей объектов [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Получение androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-get.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Чтение свойств и связей объекта [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Создание androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-create.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Создайте объект [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Удаление androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-delete.md)|Нет|Удаляет [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).|
|[Обновление androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-update.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Обновление свойств объекта [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|

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
|packageId|String|Идентификатор пакета. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appIdentifier|String|Имя удостоверения. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|usedLicenseCount|Int32|Количество используемых лицензий VPP. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|totalLicenseCount|Int32|Общее количество лицензий VPP. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appStoreUrl|String|URL-адрес приложения Play for Work Store. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|isPrivate|Логический|Указывает, доступно ли приложение только пользователям данного предприятия. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|isSystemApp|Логический|Указывает, является ли приложение предустановленным системным приложением. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appTracks|[Коллекция androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)|Дорожки, видимые для этого предприятия. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|supportsOemConfig|Логическое|Поддерживает ли это приложение политику OEMConfig. Наследуется от [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Отношения|[Коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreWebApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "String",
  "appIdentifier": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "appStoreUrl": "String",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "String",
      "trackAlias": "String"
    }
  ],
  "supportsOemConfig": true
}
```




