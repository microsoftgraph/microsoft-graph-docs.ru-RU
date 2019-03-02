---
title: Тип ресурса Пайменттермс
description: Объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365642"
---
# <a name="paymentterms-resource-type"></a>Тип ресурса Пайменттермс
Представляет термин платежа в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                      | Возвращаемый тип|Описание            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[Получение Пайменттермс](../api/dynamics-paymentterms-get.md)      |Пайменттермс|Получение объекта условий оплаты.   |
|[POST Пайменттермс](../api/dynamics-create-paymentterms.md)  |Пайменттермс|Создайте объект формулы оплаты.|
|[Исправление Пайменттермс](../api/dynamics-paymentterms-update.md) |Пайменттермс|Обновление объекта условий оплаты.|
|[Удаление Пайменттермс](../api/dynamics-paymentterms-delete.md)|Нет        |Удаление объекта условий оплаты.|

## <a name="properties"></a>Свойства
| Свойство                     | Тип     |Описание                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |Уникальный идентификатор Пайменттермс. Не редактируемые.           |
|code                          |строка  |Определяет код условия платежа.                           |
|displayName                   |строка  |Задает отображаемое имя условия платежа.                   |
|Дуедатекалкулатион            |строка  |Указывает формулу, используемую для расчета даты, на которую необходимо выполнить платеж.|
|Дискаунтдатекалкулатион       |строка  |Указывает формулу, используемую для расчета даты, которую необходимо выполнить для получения скидки.|
|Дискаунтперцент               |числе |Указывает процент скидки, который применяется для раннего платежа по сумме накладной.|
|Калкулатедискаунтонкредитмемос|boolean |Указывает, следует ли применять скидку к кредитовым нотам. **Значение true** указывает, что будет задана скидка, **значение false** указывает, что скидка не будет задана.|
|lastModifiedDateTime          |отличным|Дата и время последнего изменения Пайменттермс. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление объекта Пайменттермс в формате JSON.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
