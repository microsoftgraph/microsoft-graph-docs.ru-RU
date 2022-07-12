---
title: Тип ресурса workPosition
description: Тип ресурса workPosition
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people-and-workplace-intelligence
doc_type: resourcePageType
ms.openlocfilehash: e26e9d5a4d48cb2b1186b1ea69e4b462a8ef93a4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730583"
---
# <a name="workposition-resource-type"></a>Тип ресурса workPosition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о рабочих позициях, связанных с профилем [пользователя](profile.md).

Этот тип ресурса наследуется от [itemFacet](itemfacet.md).


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Позиции списка](../api/profile-list-positions.md)|[Коллекция workPosition](../resources/workposition.md)|Получение ресурсов workPosition из свойства навигации positions.|
|[Создание рабочей позиции](../api/profile-post-positions.md)|[workPosition](../resources/workposition.md)|Создайте объект workPosition.|
|[Получение рабочей позиции](../api/workposition-get.md)|[workPosition](../resources/workposition.md)|Чтение свойств и связей объекта [workPosition](../resources/workposition.md) .|
|[Обновление рабочей позиции](../api/workposition-update.md)|[workPosition](../resources/workposition.md)|Обновление свойств объекта [workPosition](../resources/workposition.md) .|
|[Удаление рабочей позиции](../api/workposition-delete.md)|Нет|Удаляет объект [workPosition](../resources/workposition.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется [от itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Категории, связанные с этой позицией пользователем.|
|Коллег|[Коллекция relatedPerson](../resources/relatedperson.md)|Коллеги, связанные с этой позицией.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и (или) приложения, создавшего сущность. Наследуется [от itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания сущности. Наследуется [от itemFacet](../resources/itemfacet.md).|
|Детали|[positionDetail](../resources/positiondetail.md)|Содержит подробные сведения о позиции. |
|id|String|Идентификатор, используемый для индивидуального адреса сущности. Наследуется [от сущности](../resources/entity.md)|
|Вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если сущность выводится при создании или изменении приложения. Наследуется [от itemFacet](../resources/itemfacet.md).|
|isCurrent|Логический|Указывает, является ли позиция текущей.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и (или) приложения, которые в последний раз изменяли сущность. Наследуется [от itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания сущности. Наследуется [от itemFacet](../resources/itemfacet.md).|
|manager|[relatedPerson](../resources/relatedperson.md)|Содержит сведения о руководителе пользователя в этой позиции.|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы из другой службы. Наследуется [от itemFacet](../resources/itemfacet.md).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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

