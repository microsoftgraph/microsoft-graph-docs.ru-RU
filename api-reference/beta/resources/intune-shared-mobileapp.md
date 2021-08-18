---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b606226e62e7eccfc65bb3c19fd359fff4a2c7161506404aa6eed09c481e2f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54214917"
---
# <a name="mobileapp-resource-type"></a>Тип ресурса mobileApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileApps](../api/intune-shared-mobileapp-list.md)|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Список свойств и связей объектов [mobileApp](../resources/intune-shared-mobileapp.md).|
|[Получение объекта mobileApp](../api/intune-shared-mobileapp-get.md)|[mobileApp](../resources/intune-shared-mobileapp.md)|Чтение свойств и связей объекта [mobileApp](../resources/intune-shared-mobileapp.md).|
|**Приложения**|
|[Действие assign](../api/intune-shared-mobileapp-assign.md)|Нет|Н/Д|
|[функция getMobileAppCount](../api/intune-shared-mobileapp-getmobileappcount.md)|Int64|Пока не задокументировано.|
|[функция getTopMobileApps](../api/intune-shared-mobileapp-gettopmobileapps.md)|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Пока не задокументировано.|
|[действие updateRelationships](../api/intune-shared-mobileapp-updaterelationships.md)|Нет|Н/Д|
|[функция getRelatedAppStates](../api/intune-shared-mobileapp-getrelatedappstates.md)|[коллекция mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)|Пока не задокументировано.|
|**Набор политик**|
|[действие hasPayloadLinks](../api/intune-shared-mobileapp-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Администратор предоставил или импортировал название приложения.|
|description|String|Описание приложения.|
|publisher|String|Издатель приложения.|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Большой значок, отображается в сведениях о приложении и используется для отправки значка.|
|createdDateTime|DateTimeOffset|Дата и время создания приложения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения.|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором.|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности.|
|informationUrl|String|URL-адрес с дополнительными сведениями.|
|owner|String|Владелец приложения.|
|developer|String|Разработчик приложения.|
|notes|String|Заметки для приложения.|
|uploadState|Int32|Состояние загрузки.|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение не может быть назначено, если оно не опубликовано. Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению по крайней мере одна группа.|
|roleScopeTagIds|Коллекция String|Список ids тегов области для этого мобильного приложения.|
|dependentAppCount|Int32|Общее число зависимостей, которые имеет детское приложение.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения.|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения.|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения.|
|deviceStatuses|[коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояния установки для этого мобильного приложения.|
|userStatuses|[коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояния установки для этого мобильного приложения.|
|отношения|[коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Список отношений для этого мобильного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "dependentAppCount": 1024
}
```




