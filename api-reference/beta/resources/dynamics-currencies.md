---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e986777d277e84246104561e5e275d7508b41b7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504736"
---
# <a name="currencies-resource-type"></a>Тип ресурса "валюты"

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет валюту, используемую в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод                                                  |Возвращаемый тип|Описание       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Получение валют](../api/dynamics-currencies-get.md)      |друг |Получение валюты.   |
|[Разноска денежных единиц](../api/dynamics-create-currencies.md)  |друг |Создание денежной единицы.|
|[Единицы обновления](../api/dynamics-currencies-update.md) |друг |Обновление денежной единицы.|
|[Удаление валют](../api/dynamics-currencies-delete.md)|нет       |Удаление денежной единицы.|

## <a name="properties"></a>Свойства
| Свойство              | Тип   |Описание                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |Уникальный идентификатор валюты. Не редактируемые.                  |
|code                   |string  |Указывает код валюты.                                  |
|displayName            |string  |Задает отображаемое имя денежной единицы.                          |
|знаки                 |строка  |Указывает символ валюты, который будет отображаться при проверке.|
|амаунтдеЦималплацес    |строка  |Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.|
|амаунтраундингпреЦисион|числе |Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.|
|lastModifiedDateTime   |datetime|Дата и время последнего изменения валюты. Только для чтения.       |  


## <a name="relationships"></a>Связи
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

