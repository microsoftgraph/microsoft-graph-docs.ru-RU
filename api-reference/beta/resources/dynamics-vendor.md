---
title: Тип ресурса "поставщики"
description: Объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a2102a77748ebef8267792a887a522fa716619ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040049"
---
# <a name="vendors-resource-type"></a>Тип ресурса "поставщики"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщика в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение поставщиков](../api/dynamics-vendor-get.md)|поставщиков|Возвращает объект Vendor.|
|[Учет поставщиков](../api/dynamics-create-vendor.md)|поставщиков|Создает объект Vendor.|
|[Поставщики обновлений](../api/dynamics-vendor-update.md)|поставщиков|Обновляет объект Vendor.|
|[Удаление поставщика](../api/dynamics-vendor-delete.md)|Нет|Удаляет объект Vendor.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор поставщика. Не редактируемые.|
|число|string|Номер поставщика.|
|displayName|string|Отображаемое имя поставщика.|
|address|[Навигационная. посталаддресс](../resources/dynamics-complextypes.md)|Адрес поставщика.|
|phoneNumber|string|Номер телефона поставщика.|
|email|строка|Адрес электронной почты поставщика.|
|веб-сайт|string|Адрес веб-сайта поставщика.|
|таксрегистратионнумбер|string|Регистрационный номер налогоплательщика поставщика.|
|курренциид|GUID|Идентификатор кода валюты по умолчанию для поставщика.|
|курренцикоде|string|Код валюты по умолчанию для поставщика.|
|irs1099Code|string|Указывает код 1099 для поставщика. Только для США.|
|пайменттермсид|GUID|КОД условий оплаты для поставщика по умолчанию.|
|пайментмесодид|GUID|Идентификатор метода оплаты по умолчанию для поставщика.|
|такслиабле|boolean|Указывает, является ли поставщик подлежащей налогообложению.|
|заблокированных|string|Указывает, какие транзакции у поставщика, который не может быть разнесен. Допустимые значения: пусто, оплата или все|
|равномерно|decimal|Сальдо поставщика. Только для чтения.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения поставщика. Только для чтения.|  


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление поставщика в формате JSON.

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



