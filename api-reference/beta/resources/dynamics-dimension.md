---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 61666cdaf87e095707e90345128b5ad2cda47426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071360"
---
# <a name="dimensions-resource-type"></a>Тип ресурса Dimensions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет измерение в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:-------------|:-------------|:----------|
|[Получение измерений](../api/dynamics-dimension-get.md)|аналитики|Возвращает измерение.|


## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |Уникальный идентификатор элемента.|
|code                |Строка, максимальный размер 20|Код измерения.       |
|displayName         |string                 |Задает имя измерения. Это имя будет отображаться там, где используется измерение.|
|lastModifiedDateTime|datetime               |Дата и время последнего изменения измерения.|  


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



