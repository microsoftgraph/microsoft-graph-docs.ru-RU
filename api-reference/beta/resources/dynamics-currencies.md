---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 42dc5fec859aff758b2f46812a63b10f49f0498a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071369"
---
# <a name="currencies-resource-type"></a>Тип ресурса "валюты"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет валюту, используемую в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод                                                  |Возвращаемый тип|Описание       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Получение валют](../api/dynamics-currencies-get.md)      |друг |Получение валюты.   |
|[Разноска денежных единиц](../api/dynamics-create-currencies.md)  |друг |Создание денежной единицы.|
|[Единицы обновления](../api/dynamics-currencies-update.md) |друг |Обновление денежной единицы.|
|[Удаление валют](../api/dynamics-currencies-delete.md)|Нет       |Удаление денежной единицы.|

## <a name="properties"></a>Свойства
| Свойство              | Тип   |Описание                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |Уникальный идентификатор валюты. Не редактируемые.                  |
|code                   |string  |Указывает код валюты.                                  |
|displayName            |string  |Задает отображаемое имя денежной единицы.                          |
|знаки                 |string  |Указывает символ валюты, который будет отображаться при проверке.|
|амаунтдеЦималплацес    |string  |Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.|
|амаунтраундингпреЦисион|числе |Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.|
|lastModifiedDateTime   |datetime|Дата и время последнего изменения валюты. Только для чтения.       |  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление валют в формате JSON.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```



