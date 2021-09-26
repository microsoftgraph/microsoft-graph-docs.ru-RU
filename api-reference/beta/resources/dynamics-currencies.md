---
title: тип ресурса валют
description: Объект валюты в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 228f4c227cd8c0efa5f2ed6dcd885c81a2f5f9ab
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767085"
---
# <a name="currencies-resource-type"></a>тип ресурса валют

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет валюту, используемую в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод                                                  |Возвращаемый тип|Описание       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Получение валют](../api/dynamics-currencies-get.md)      |валюты |Получите валюту.   |
|[Почтовые валюты](../api/dynamics-create-currencies.md)  |валюты |Создание валюты.|
|[Валюты патчей](../api/dynamics-currencies-update.md) |валюты |Обновление валюты.|
|[Удаление валют](../api/dynamics-currencies-delete.md)|Нет       |Удаление валюты.|

## <a name="properties"></a>Свойства
| Свойство              | Тип   |Описание                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |Уникальный ID валюты. Не редактируемый.                  |
|code                   |string  |Указывает код валюты.                                  |
|displayName            |string  |Указывает имя отображения валюты.                          |
|символ                 |string  |Указывает символ этой валюты, который отображается на чеках.|
|amountDecimalPlaces    |string  |Указывает количество десятичных мест, которые система будет отображать на количествах для этой валюты.|
|amountRoundingPrecision|decimal |Указывает размер интервала, который будет использоваться при округлке сумм для этой валюты.|
|lastModifiedDateTime   |datetime|В последний раз валюта была изменена. Только для чтения.       |  


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Вот представление JSON валют.


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



