---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ba8ad750831394e2a84fab7ca87d76754838db60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012620"
---
# <a name="currencies-resource-type"></a>Тип ресурса "валюты"
Представляет валюту, используемую в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод                                                  |Возвращаемый тип|Описание       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Получение валют](../api/dynamics-currencies-get.md)      |друг |Получение валюты.   |
|[Разноска денежных единиц](../api/dynamics-create-currencies.md)  |друг |Создание денежной единицы.|
|[Единицы обновления](../api/dynamics-currencies-update.md) |друг |Обновление денежной единицы.|
|[Удаление валют](../api/dynamics-currencies-delete.md)|none       |Удаление денежной единицы.|

## <a name="properties"></a>Свойства
| Свойство              | Тип   |Описание                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |Уникальный идентификатор валюты. Не редактируемые.                  |
|code                   |string  |Указывает код валюты.                                  |
|displayName            |string  |Задает отображаемое имя денежной единицы.                          |
|знаки                 |string  |Указывает символ валюты, который будет отображаться при проверке.|
|АмаунтдеЦималплацес    |string  |Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.|
|АмаунтраундингпреЦисион|числе |Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.|
|lastModifiedDateTime   |отличным|Дата и время последнего изменения валюты. Только для чтения.       |  


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

