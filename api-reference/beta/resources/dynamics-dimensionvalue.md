---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: acb1c8d34f8ee876c39ac99d5f43feb7f9a128c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071348"
---
# <a name="dimensionvalues-resource-type"></a>Тип ресурса Дименсионвалуес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет значение измерения в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание                   |
|:-------------|:-------------|:-----------------------------|
|[Получение Дименсионвалуес](../api/dynamics-dimensionvalue-get.md)|дименсионвалуес|Возвращает объект значения измерения.|


## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор элемента.                         |
|code                |Строка, максимальный размер 20|Код значения измерения.                          |
|displayName         |string                 |Задает имя значения измерения. Это имя будет отображаться там, где используется значение измерения.|
|lastModifiedDateTime|datetime               |Дата и время последнего изменения значения измерения.|  


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```




