---
title: Тип ресурса "учетная запись"
description: Тип ресурса "учетная запись"
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 29d66809d14cfc72d43286aef801490cef20cb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057684"
---
# <a name="webaccount-resource-type"></a>Тип ресурса "учетная запись"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой [профиль](profile.md)пользователя.

Этот тип ресурса наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список учетных записей](../api/profile-list-webaccounts.md)|Коллекция [учетных записей](../resources/webaccount.md)|Получение ресурсов учетной записи службы из свойства навигации для учетных записей учетных записей.|
|[Создание учетной записи](../api/profile-post-webaccounts.md)|[Учетная запись учетной записи](../resources/webaccount.md)|Создайте новый объект учетной записи.|
|[Получение учетной записи службы](../api/webaccount-get.md)|[Учетная запись учетной записи](../resources/webaccount.md)|Чтение свойств и связей объекта веб- [учетных записей](../resources/webaccount.md) .|
|[Обновление учетной записи](../api/webaccount-update.md)|[Учетная запись учетной записи](../resources/webaccount.md)|Обновление свойств объекта [учетной записи](../resources/webaccount.md) .|
|[Удаление учетной записи службы](../api/webaccount-delete.md)|Нет|Удаляет объект [учетной записи](../resources/webaccount.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|String|Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|service|[сервицеинформатион](../resources/serviceinformation.md)| Содержит основные сведения о связанной службе. |
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|статусмессаже|String|Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано. |
|userId|String|Имя пользователя, отображаемое для учетной записи Account.  |
|webUrl|String|Содержит ссылку на профиль пользователя в облачной службе, если она существует.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webAccount",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "description": "String",
  "userId": "String",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation"
  },
  "statusMessage": "String",
  "webUrl": "String"
}
```


