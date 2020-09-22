---
title: Тип ресурса Итемфоне
description: Тип ресурса Итемфоне
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c1263f004b9c3c85621bc2cef4fe8622a7a1cb54
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033699"
---
# <a name="itemphone-resource-type"></a>Тип ресурса Итемфоне

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление телефонов](../api/profile-list-phones.md)|Коллекция [итемфоне](../resources/itemphone.md)|Получение ресурсов Итемфоне из свойства навигации phones.|
|[Создание Итемфоне](../api/profile-post-phones.md)|[итемфоне](../resources/itemphone.md)|Создание нового объекта Итемфоне.|
|[Получение Итемфоне](../api/itemphone-get.md)|[итемфоне](../resources/itemphone.md)|Чтение свойств и связей объекта [итемфоне](../resources/itemphone.md) .|
|[Обновление Итемфоне](../api/itemphone-update.md)|[итемфоне](../resources/itemphone.md)|Обновление свойств объекта [итемфоне](../resources/itemphone.md) .|
|[Удаление Итемфоне](../api/itemphone-delete.md)|Нет|Удаляет объект [итемфоне](../resources/itemphone.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|displayName|String|Понятное имя, назначенное пользователю для этого номера телефона. |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|число|String|Номер телефона, предоставленный пользователем.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|type|фонетипе|Тип номера телефона в объекте. Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.itemPhone",
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
  "displayName": "String",
  "type": "String",
  "number": "String"
}
```


