---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507219"
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
|displayName         |string                 |Задает имя значения измерения. Это имя будет отображаться там, где используется значение измерения.|
|lastModifiedDateTime|отличным               |Дата и время последнего изменения значения измерения.|  


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


