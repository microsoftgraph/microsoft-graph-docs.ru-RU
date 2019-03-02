---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366629"
---
# <a name="currencies-resource-type"></a>Тип ресурса "валюты"
Представляет валюту, используемую в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод                                                  |Возвращаемый тип|Описание       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Получение валют](../api/dynamics-currencies-get.md)      |друг |Получение валюты.   |
|[Разноска денежных единиц](../api/dynamics-create-currencies.md)  |друг |Создание денежной единицы.|
|[Единицы обновления](../api/dynamics-currencies-update.md) |друг |Обновление денежной единицы.|
|[Удаление денежных единиц](../api/dynamics-currencies-delete.md)|Нет       |Удаление денежной единицы.|

## <a name="properties"></a>Свойства
| Свойство              | Тип   |Описание                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |Уникальный идентификатор валюты. Не редактируемые.                  |
|code                   |строка  |Указывает код валюты.                                  |
|displayName            |строка  |Задает отображаемое имя денежной единицы.                          |
|знаки                 |строка  |Указывает символ валюты, который будет отображаться при проверке.|
|АмаунтдеЦималплацес    |строка  |Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.|
|АмаунтраундингпреЦисион|числе |Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.|
|lastModifiedDateTime   |отличным|Дата и время последнего изменения валюты. Только для чтения.       |  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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

