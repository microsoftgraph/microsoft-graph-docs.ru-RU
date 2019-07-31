---
title: Тип ресурса "поставщики"
description: Объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7c0609d96f6d97503faf5c5251d3641979a4f6e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972854"
---
# <a name="vendors-resource-type"></a>Тип ресурса "поставщики"
Представляет поставщика в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение поставщиков](../api/dynamics-vendor-get.md)|поставщиков|Возвращает объект Vendor.|
|[Учет поставщиков](../api/dynamics-create-vendor.md)|поставщиков|Создает объект Vendor.|
|[Поставщики обновлений](../api/dynamics-vendor-update.md)|поставщиков|Обновляет объект Vendor.|
|[Удаление поставщика](../api/dynamics-vendor-delete.md)|none|Удаляет объект Vendor.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор поставщика. Не редактируемые.|
|число|string|Номер поставщика.|
|displayName|string|Отображаемое имя поставщика.|
|address|[Навигационная. Посталаддресс](../resources/dynamics-complextypes.md)|Адрес поставщика.|
|phoneNumber|string|Номер телефона поставщика.|
|email|string|Адрес электронной почты поставщика.|
|веб-сайт|string|Адрес веб-сайта поставщика.|
|Таксрегистратионнумбер|string|Регистрационный номер налогоплательщика поставщика.|
|Курренциид|GUID|Идентификатор кода валюты по умолчанию для поставщика.|
|Курренцикоде|string|Код валюты по умолчанию для поставщика.|
|irs1099Code|string|Указывает код 1099 для поставщика. Только для США.|
|Пайменттермсид|GUID|КОД условий оплаты для поставщика по умолчанию.|
|Пайментмесодид|GUID|Идентификатор метода оплаты по умолчанию для поставщика.|
|Такслиабле|boolean|Указывает, является ли поставщик подлежащей налогообложению.|
|заблокированных|string|Указывает, какие транзакции у поставщика, который не может быть разнесен. Допустимые значения: пусто, оплата или все|
|равномерно|числе|Сальдо поставщика. Только для чтения.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения поставщика. Только для чтения.|  


## <a name="relationships"></a>Отношения
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

