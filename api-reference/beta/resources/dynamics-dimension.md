---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5bd5382ae020baaf726db53f9252c4d3498833ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973627"
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
|displayName         |string                 |Задает имя измерения. Это имя будет отображаться там, где используется измерение.|
|lastModifiedDateTime|отличным               |Дата и время последнего изменения измерения.|  


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

