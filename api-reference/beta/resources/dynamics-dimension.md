---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ed7c7a389778e651af8d2c11c53277a27e022ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504540"
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

