---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 368fc28f7bd46d8d5385b6e6041cd82255e0271f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504141"
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


