---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365572"
---
# <a name="dimensions-resource-type"></a>Тип ресурса Dimensions
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
|displayName         |строка                 |Задает имя измерения. Это имя будет отображаться там, где используется измерение.|
|lastModifiedDateTime|отличным               |Дата и время последнего изменения измерения.|  


## <a name="json-representation"></a>Описание в формате JSON

Ниже представлено описание ресурса в формате JSON.


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

