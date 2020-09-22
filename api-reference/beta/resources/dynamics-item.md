---
title: Тип ресурса Items
description: Объект item в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 89ccee3123fc3f0fc04b620e5b3528f4a253d1fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058454"
---
# <a name="items-resource-type"></a>Тип ресурса Items

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элемент в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                      |Возвращаемый тип|Описание |
|:--------------------------------------------|:----------|:-----------|
|[Получение элементов](../api/dynamics-item-get.md)      |items     |Возвращает объект Item.   |
|[Размещение элементов](../api/dynamics-create-item.md)  |items     |Создает объект Item.|
|[Элемент Patch](../api/dynamics-item-update.md)  |items     |Обновляет объект Item.|
|[Удаление элементов](../api/dynamics-item-delete.md)|Нет      |Удаляет объект Item.|

## <a name="properties"></a>Свойства
| Свойство           | Тип |Описание                                          |
|:-------------------|:-------|:----------------------------------------------------|
|id                  |GUID    |Уникальный идентификатор элемента. Не редактируемые.             |
|число              |string  |Номер элемента.                                     |
|displayName         |string  |Задает описание элемента.                 |
|type                |числовых |Тип запасов для элемента. 1 = складская номенклатура, 2 = сервисный товар. Это обязательное свойство.|
|заблокированных             |boolean |Указывает, что транзакции с элементом не могут быть опубликованы, например, потому что элемент находится в карантине. Имеет значение **true**, если элемент блокируется.|
|басеунитофмеасуреид |GUID    |Задает идентификатор единицы измерения.             |
|басеунитофмеасуре   |[Навигационная. унитофмеасуре](../resources/dynamics-complextypes.md)|Задает единицу измерения, в которой хранится элемент в перечне.|
|GTIN                |числовых |Это номер глобального торгового элемента.                |
|итемкатегорид      |GUID |Указывает категорию, к которой принадлежит элемент. Категории элементов также содержат назначенные атрибуты элемента.|
|inventory           |числе |Указывает, сколько единиц товара, таких как штуки, коробки или г., находится на складе. Только для чтения.|
|unitPrice           |числе |Указывает цену для одной единицы элемента в указанной валюте.|
|прицеинклудестакс    |boolean |Указывает, что цена включает налог. Имеет значение **true**, если цена включает налог.|
|униткост            |числе |Указывает затраты на единицу измерения элемента.             |
|таксграупид          |GUID    |Указывает идентификатор налоговой группы для элемента.      |
|таксграупкоде        |числовых |Группа налогов представляет группу складских элементов или ресурсов, которые могут быть идентичными налоговым условиям.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения элемента. Только для чтения.  |  


## <a name="relationships"></a>Связи
Налоговая группа (Таксграупкоде) должна существовать в таблице налоговой группы.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```




