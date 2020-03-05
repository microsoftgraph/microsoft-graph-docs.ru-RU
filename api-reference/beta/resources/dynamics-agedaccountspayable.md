---
title: Тип ресурса Ажедаккаунтспайабле
description: Объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9a8dc7eed4bdbcc39a04f55996e11b6d9dc6da1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505170"
---
# <a name="agedaccountspayable-resource-type"></a>Тип ресурса Ажедаккаунтспайабле

Пространство имен: Microsoft. Graph

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
|вендорнумбер   |строка    |Указывает номер поставщика.                  |
|name           |string    |Указывает имя поставщика.                    |
|курренцикоде   |строка    |Задает валюту.                     |
|баланцедуе     |числовых   |Указывает общее сальдо, которое связано с поставщиком.|
|куррентамаунт  |числовых   |Указывает баланс перед первым периодом распределения по срокам.|
|period1Amount  |числовых   |Указывает баланс в первом периоде распределения по срокам.|
|period2Amount  |числовых   |Указывает баланс во втором периоде распределения по срокам.|
|period3Amount  |числовых   |Указывает баланс в третьем периоде распределения по срокам.|
|ажедасофдате   |date|Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.|
|периодленгсфилтер|строка |Указывает длину периодов. Допустимые значения для единиц времени: D, WD, W, M, Q или Y. C, то есть текущая единица времени на основе даты может быть указана в качестве префикса для единицы времени.|


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
