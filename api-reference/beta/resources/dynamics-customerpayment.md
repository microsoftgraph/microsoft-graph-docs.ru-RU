---
title: Тип ресурса Кустомерпайментс
description: Объект платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bd990ea9778ada7d43c9b8192d77cf8af618909b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504638"
---
# <a name="customerpayments-resource-type"></a>Тип ресурса Кустомерпайментс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет платеж клиента в Dynamics 365 Business Central. Клиентская оплата вводится в виде строки в журнале платежей клиента.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Кустомерпайментс](../api/dynamics-customerpayment-get.md)|кустомерпайментс|Возвращает платеж клиента.|
|[POST Кустомерпайментс](../api/dynamics-create-customerpayment.md)|кустомерпайментс|Создает платеж клиента.|
|[Исправление Кустомерпайментс](../api/dynamics-customerpayment-update.md)|кустомерпайментс|Обновляет платеж клиента.|
|[Удаление Кустомерпайментс](../api/dynamics-customerpayment-delete.md)|Нет|Удаляет платеж клиента.|

## <a name="properties"></a>Свойства
| Свойство     | Тип    |Описание|
|:-------------|:--------|:----------|
|id|GUID|Уникальный идентификатор платежа клиента. Не редактируемые.|
|жаурналдисплайнаме|string|Журнал платежей клиента, в котором запись платежа является строкой.|
|lineNumber|целое|Номер платежа клиента.|
|customerId|GUID|Уникальный идентификатор клиента, с которым связана оплата.|
|кустомернумбер|Строка, максимальный размер 20|Номер клиента, с которым связана оплата.|
|contactId|Строка, максимальный размер 250|Идентификатор контакта Exchange для данного клиента. Если идентификатор клиента не указан, мы будем использовать идентификатор контакта, чтобы найти его.|
|постингдате|date|Дата, когда выполняется разноска платежа клиента.|
|документнумбер|Строка, максимальный размер 20|Указывает номер документа для платежа клиента.|
|екстерналдокументнумбер|Строка, максимальный размер 20|Указывает номер внешнего документа для платежа клиента.|
|отступ|числе|Указывает общую сумму (включая НДС), из которой состоит платеж клиента.|
|апплиестоинвоицеид|GUID|Уникальный идентификатор счета, с которым связана оплата.|
|апплиестоинвоиценумбер|Строка, максимальный размер 20|Номер счета, с которым связана оплата.|
|description|Строка, максимальный размер 50|Описание платежа клиента, предоставленное пользователем или созданным пользователем.|
|comment|Строка, максимальный размер 250|Указанный пользователем комментарий к платежу клиента.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения платежа клиента. Только для чтения.|


## <a name="relationships"></a>Связи
Платеж клиента — это вложенная страница журнала платежей клиента. Прямой доступ к нему невозможен.

Платеж клиента может быть "родительским объектом" строк измерения.

Клиент (customerId) должен существовать в таблице Customers (клиенты).

Счет (Апплиестоинвоицеид) должен существовать в таблице "счета продаж".


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

