---
title: Тип ресурса Воркпоситион
description: Тип ресурса Воркпоситион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d812efcff378d5ef58f7d49fe318768e2efdb31e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046099"
---
# <a name="workposition-resource-type"></a>Тип ресурса Воркпоситион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о должностных единицах, связанных с [профилем](profile.md)пользователя.

Этот тип ресурса наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Позиции списка](../api/profile-list-positions.md)|Коллекция [воркпоситион](../resources/workposition.md)|Получение ресурсов Воркпоситион из свойства навигации Positions.|
|[Создание Воркпоситион](../api/profile-post-positions.md)|[воркпоситион](../resources/workposition.md)|Создание нового объекта Воркпоситион.|
|[Получение Воркпоситион](../api/workposition-get.md)|[воркпоситион](../resources/workposition.md)|Чтение свойств и связей объекта [воркпоситион](../resources/workposition.md) .|
|[Обновление Воркпоситион](../api/workposition-update.md)|[воркпоситион](../resources/workposition.md)|Обновление свойств объекта [воркпоситион](../resources/workposition.md) .|
|[Удаление Воркпоситион](../api/workposition-delete.md)|Нет|Удаляет объект [воркпоситион](../resources/workposition.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|Строка|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Категории, связанные с этим положением пользователя.|
|коллег|Коллекция [релатедперсон](../resources/relatedperson.md)|Коллеги, связанные с этой позицией.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|описаны|[поситиондетаил](../resources/positiondetail.md)|Содержит подробные сведения о позиции. |
|id|Строка|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|по току|Boolean|Указывает, является ли должность текущей.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|manager|[релатедперсон](../resources/relatedperson.md)|Содержит сведения о руководителе пользователя в этой позиции.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workPosition",
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
  "categories": [
    "String"
  ],
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "manager": {
    "@odata.type": "microsoft.graph.relatedPerson"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "isCurrent": "Boolean"
}
```

