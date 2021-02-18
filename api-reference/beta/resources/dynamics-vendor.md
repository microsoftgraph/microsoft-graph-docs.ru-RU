---
title: Тип ресурса vendors
description: Объект поставщика в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0848b6fbb67964faa9565f2ed95120f563c71f53
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293073"
---
# <a name="vendors-resource-type"></a>Тип ресурса vendors

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получить поставщиков](../api/dynamics-vendor-get.md)|поставщики|Получает объект поставщика.|
|[Поставщики post](../api/dynamics-create-vendor.md)|поставщики|Создает объект поставщика.|
|[Поставщики исправлений](../api/dynamics-vendor-update.md)|поставщики|Обновляет объект поставщика.|
|[Удаление поставщика](../api/dynamics-vendor-delete.md)|Нет|Удаляет объект поставщика.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный ИД поставщика. Нередактируемое.|
|число|Строка|Номер поставщика.|
|displayName|string|Отображаемая фамилия поставщика.|
|address|[NAV. PostalAddress](../resources/dynamics-complextypes.md)|Адрес поставщика.|
|phoneNumber|Строка|Номер телефона поставщика.|
|email|строка|Адрес электронной почты поставщика.|
|веб-сайт|Строка|Адрес веб-сайта поставщика.|
|taxRegistrationNumber|Строка|Номер регистрации налога поставщика.|
|currencyId|GUID|Код валюты по умолчанию для поставщика.|
|currencyCode|Строка|Код валюты по умолчанию для поставщика.|
|irs1099Code|Строка|Указывает код 1099 для поставщика. Только для США.|
|paymentTermsId|GUID|ИД условий оплаты по умолчанию для поставщика.|
|paymentMethodId|GUID|ИД метода оплаты по умолчанию для поставщика.|
|taxLiable|boolean|Указывает, несет ли поставщик ответственность за налоги.|
|blocked|Строка|Указывает, какие транзакции с поставщиком не могут быть опубликованы. Accepted values are blank, Payment or All|
|balance|decimal|Баланс поставщика. Только для чтения.|
|lastModifiedDateTime|datetime|Дата последнего изменения поставщика. Только для чтения.|  


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vendor"
}-->

Вот представление поставщика в JSON.

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}
```



