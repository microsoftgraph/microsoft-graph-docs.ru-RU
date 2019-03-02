---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365320"
---
# <a name="dimensionvalues-resource-type"></a>Тип ресурса Дименсионвалуес
Представляет значение измерения в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание                   |
|:-------------|:-------------|:-----------------------------|
|[Получение Дименсионвалуес](../api/dynamics-dimensionvalue-get.md)|Дименсионвалуес|Возвращает объект значения измерения.|


## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор элемента.                         |
|code                |Строка, максимальный размер 20|Код значения измерения.                          |
|displayName         |строка                 |Задает имя значения измерения. Это имя будет отображаться там, где используется значение измерения.|
|lastModifiedDateTime|отличным               |Дата и время последнего изменения значения измерения.|  


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


