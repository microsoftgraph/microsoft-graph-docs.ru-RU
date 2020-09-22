---
title: Тип ресурса Итемфацет
description: Тип ресурса Итемфацет
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ff186b8b78e0070b5f92efa1858ef8d15d51c59f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021436"
---
# <a name="itemfacet-resource-type"></a>Тип ресурса Итемфацет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет абстрактный базовый тип, от которого наследуются все типы ресурсов в наборе EntitySet [профиля](profile.md) .

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|алловедаудиенцес|Аудитории, которые могут просматривать значения, содержащиеся в связанном объекте. Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность.|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект.|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений в сущности при синхронизации от другой службы.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemFacet",
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
  }
}
```



