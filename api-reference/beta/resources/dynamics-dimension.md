---
title: тип ресурса размеров
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: db1a243a9f7eabb8436a6f1ca2b64fe5b74508b5
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767078"
---
# <a name="dimensions-resource-type"></a>Тип ресурса Dimensions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет измерение в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:-------------|:-------------|:----------|
|[Получить размеры](../api/dynamics-dimension-get.md)|размер|Получает измерение.|


## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |Уникальный ID элемента.|
|code                |строка, максимальный размер 20|Код измерения.       |
|displayName         |string                 |Указывает имя измерения. Это имя появится там, где используется измерение.|
|lastModifiedDateTime|datetime               |В последнее время измерение было изменено.|  


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



