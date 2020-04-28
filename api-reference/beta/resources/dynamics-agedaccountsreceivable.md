---
title: Тип ресурса Ажедаккаунтсрецеивабле
description: Объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 82d6ead5d41820f827f58d5a9069744e1b2ac49d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505163"
---
# <a name="agedaccountsreceivable-resource-type"></a>Тип ресурса Ажедаккаунтсрецеивабле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект Ажедаккаунтсрецеивабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи клиента.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Ажедаккаунтсрецеивабле](../api/dynamics-agedaccountsreceivable-get.md)|ажедаккаунтсрецеивабле|Получение объекта Ажедаккаунтсрецеивабле|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание                                  |
|:---------------|:--------|:--------------------------------------------|
|customerId      |GUID     |Уникальный идентификатор клиента.                   |
|кустомернумбер  |string   |Указывает номер клиента.                 |
|name            |string   |Указывает имя клиента.                   |
|курренцикоде    |string   |Задает валюту.                      |
|баланцедуе      |числовых  |Указывает общее сальдо клиента.      |
|куррентамаунт   |числовых  |Указывает баланс для текущего периода распределения по срокам.|
|period1Amount   |числовых  |Указывает баланс в первом периоде распределения по срокам. |
|period2Amount   |числовых  |Указывает баланс во втором периоде распределения по срокам.|
|period3Amount   |числовых  |Указывает баланс в третьем периоде распределения по срокам. |
|ажедасофдате    |date     |Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.|
|периодленгсфилтер|string |Указывает длину периодов. Допустимые единицы времени: D, WD, W, M, Q и Y. C, то есть текущая единица времени на основе даты может указываться в качестве префикса для единицы времени.|


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```


