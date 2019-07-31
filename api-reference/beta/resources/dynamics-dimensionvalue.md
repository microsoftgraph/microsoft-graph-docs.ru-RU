---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af7ba3b49051a4e89fcdf2a4a408a1f72fc547ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973617"
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


