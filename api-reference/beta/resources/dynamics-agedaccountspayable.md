---
title: Тип ресурса Ажедаккаунтспайабле
description: Объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: dfbedf2e3f47d287842773d5da1c4e79ed126695
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058468"
---
# <a name="agedaccountspayable-resource-type"></a>Тип ресурса Ажедаккаунтспайабле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект Ажедаккаунтспайабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи поставщика.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Ажедаккаунтспайабле](../api/dynamics-agedaccountspayable-get.md)|ажедаккаунтспайабле|Получение объекта Ажедаккаунтспайабле|

## <a name="properties"></a>Свойства
| Свойство      | Тип     |Описание                                 |
|:--------------|:---------|:-------------------------------------------|
|Поставщика       |GUID      |Уникальный идентификатор поставщика.                    |
|вендорнумбер   |string    |Указывает номер поставщика.                  |
|name           |string    |Указывает имя поставщика.                    |
|курренцикоде   |string    |Задает валюту.                     |
|баланцедуе     |числовых   |Указывает общее сальдо, которое связано с поставщиком.|
|куррентамаунт  |числовых   |Указывает баланс перед первым периодом распределения по срокам.|
|period1Amount  |числовых   |Указывает баланс в первом периоде распределения по срокам.|
|period2Amount  |числовых   |Указывает баланс во втором периоде распределения по срокам.|
|period3Amount  |числовых   |Указывает баланс в третьем периоде распределения по срокам.|
|ажедасофдате   |date|Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.|
|периодленгсфилтер|string |Указывает длину периодов. Допустимые значения для единиц времени: D, WD, W, M, Q или Y. C, то есть текущая единица времени на основе даты может быть указана в качестве префикса для единицы времени.|


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
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


