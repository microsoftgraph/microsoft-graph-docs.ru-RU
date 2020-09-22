---
title: Тип ресурса Пайменттермс
description: Объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 1e9e7951da79d524002f004410ef6939d7be5b99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027085"
---
# <a name="paymentterms-resource-type"></a>Тип ресурса Пайменттермс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет термин платежа в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                      | Возвращаемый тип|Описание            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[Получение Пайменттермс](../api/dynamics-paymentterms-get.md)      |пайменттермс|Получение объекта условий оплаты.   |
|[POST Пайменттермс](../api/dynamics-create-paymentterms.md)  |пайменттермс|Создайте объект формулы оплаты.|
|[Исправление Пайменттермс](../api/dynamics-paymentterms-update.md) |пайменттермс|Обновление объекта условий оплаты.|
|[Удаление Пайменттермс](../api/dynamics-paymentterms-delete.md)|Нет        |Удаление объекта условий оплаты.|

## <a name="properties"></a>Свойства
| Свойство                     | Тип     |Описание                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |Уникальный идентификатор Пайменттермс. Не редактируемые.           |
|code                          |string  |Определяет код условия платежа.                           |
|displayName                   |string  |Задает отображаемое имя условия платежа.                   |
|дуедатекалкулатион            |string  |Указывает формулу, используемую для расчета даты, на которую необходимо выполнить платеж.|
|дискаунтдатекалкулатион       |string  |Указывает формулу, используемую для расчета даты, которую необходимо выполнить для получения скидки.|
|дискаунтперцент               |числе |Указывает процент скидки, который применяется для раннего платежа по сумме накладной.|
|калкулатедискаунтонкредитмемос|boolean |Указывает, следует ли применять скидку к кредитовым нотам. **Значение true** указывает, что будет задана скидка, **значение false** указывает, что скидка не будет задана.|
|lastModifiedDateTime          |datetime|Дата и время последнего изменения Пайменттермс. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

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


