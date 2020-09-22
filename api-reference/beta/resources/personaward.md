---
title: Тип ресурса Персонавард
description: Тип ресурса Персонавард
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cf9656eee15c2f537f7ba7e2727ce406850878c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997948"
---
# <a name="personaward-resource-type"></a>Тип ресурса Персонавард

Пространство имен: microsoft.graph

Представляет награду, связанную с [профилем](../resources/profile.md)пользователя.

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список вознаграждений](../api/profile-list-awards.md)|Коллекция [персонавард](../resources/personaward.md)|Получение ресурсов Персонавард из свойства навигации "награды".|
|[Создание Персонавард](../api/profile-post-awards.md)|[персонавард](../resources/personaward.md)|Создание нового объекта Персонавард.|
|[Получение Персонавард](../api/personaward-get.md)|[персонавард](../resources/personaward.md)|Чтение свойств и связей объекта [персонавард](../resources/personaward.md) .|
|[Обновление Персонавард](../api/personaward-update.md)|[персонавард](../resources/personaward.md)|Обновление свойств объекта [персонавард](../resources/personaward.md) .|
|[Удаление Персонавард](../api/personaward-delete.md)|Нет|Удаляет объект [персонавард](../resources/personaward.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|String|Дескприптион вознаграждения или почетной грамоты. |
|displayName|String|Название вознаграждения или соблюдается. |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|иссуеддате|Дата|Дата предоставления вознаграждения или почетной грамоты. |
|иссуингаусорити|String|Орган, которому предоставлена премия или соблюдается.  |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|thumbnailUrl|String|URL-адрес, ссылающийся на эскиз вознаграждения или соблюдается.  |
|webUrl|String|URL-адрес, ссылающийся на награду или соблюдать. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAward",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAward",
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
  "displayName": "String",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


