---
title: Тип ресурса androidStoreApp
description: Содержит свойства, в том числе унаследованные, для приложений из магазина Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3587088d4bcebcef4e68e3abf2549a0ae1d79477
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161630"
---
# <a name="androidstoreapp-resource-type"></a>Тип ресурса androidStoreApp

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, в том числе унаследованные, для приложений из магазина Android.


Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов androidStoreApp](../api/intune-apps-androidstoreapp-list.md)|Коллекция объектов [androidStoreApp](../resources/intune-apps-androidstoreapp.md)|Список свойств и связей объектов [androidStoreApp](../resources/intune-apps-androidstoreapp.md).|
|[Получение объекта androidStoreApp](../api/intune-apps-androidstoreapp-get.md)|[androidStoreApp](../resources/intune-apps-androidstoreapp.md)|Список свойств и связей объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).|
|[Создание объекта androidStoreApp](../api/intune-apps-androidstoreapp-create.md)|[androidStoreApp](../resources/intune-apps-androidstoreapp.md)|Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).|
|[Удаление объекта androidStoreApp](../api/intune-apps-androidstoreapp-delete.md)|Нет|Удаление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).|
|[Обновление объекта androidStoreApp](../api/intune-apps-androidstoreapp-update.md)|[androidStoreApp](../resources/intune-apps-androidstoreapp.md)|Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).|

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
|uploadState|Int32|Состояние отправки. Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` . Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md) Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению хотя бы одна группа. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция String|Список ид тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|dependentAppCount|Int32|Общее количество зависимостей, которые есть у этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersedingAppCount|Int32|Общее количество приложений, которые это приложение напрямую или косвенно перемежает. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersededAppCount|Int32|Общее количество приложений, которые это приложение напрямую или косвенно перемежает. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|packageId|String|Идентификатор пакета.|
|appIdentifier|String|Имя удостоверения.|
|appStoreUrl|String|URL-адрес магазина приложений для Android.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояния установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|userStatuses|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояния установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|relationships|[Коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




