---
title: Тип ресурса Пайменттермс
description: Объект условий оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: cf6917b724f9e35735d63d1cda13c01d6f9003bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503602"
---
# <a name="paymentterms-resource-type"></a>Тип ресурса Пайменттермс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет термин платежа в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                      | Возвращаемый тип|Описание            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[Получение Пайменттермс](../api/dynamics-paymentterms-get.md)      |пайменттермс|Получение объекта условий оплаты.   |
|[POST Пайменттермс](../api/dynamics-create-paymentterms.md)  |пайменттермс|Создайте объект формулы оплаты.|
|[Исправление Пайменттермс](../api/dynamics-paymentterms-update.md) |пайменттермс|Обновление объекта условий оплаты.|
|[Удаление Пайменттермс](../api/dynamics-paymentterms-delete.md)|нет        |Удаление объекта условий оплаты.|

## <a name="properties"></a>Свойства
| Свойство                     | Тип     |Описание                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |Уникальный идентификатор Пайменттермс. Не редактируемые.           |
|code                          |string  |Определяет код условия платежа.                           |
|displayName                   |string  |Задает отображаемое имя условия платежа.                   |
|дуедатекалкулатион            |строка  |Указывает формулу, используемую для расчета даты, на которую необходимо выполнить платеж.|
|дискаунтдатекалкулатион       |строка  |Указывает формулу, используемую для расчета даты, которую необходимо выполнить для получения скидки.|
|дискаунтперцент               |числе |Указывает процент скидки, который применяется для раннего платежа по сумме накладной.|
|калкулатедискаунтонкредитмемос|boolean |Указывает, следует ли применять скидку к кредитовым нотам. **Значение true** указывает, что будет задана скидка, **значение false** указывает, что скидка не будет задана.|
|lastModifiedDateTime          |datetime|Дата и время последнего изменения Пайменттермс. Только для чтения.|  


## <a name="relationships"></a>Связи
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
