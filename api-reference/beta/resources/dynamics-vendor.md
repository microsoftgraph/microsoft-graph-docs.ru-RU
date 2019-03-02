---
title: Тип ресурса "поставщики"
description: Объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365663"
---
# <a name="vendors-resource-type"></a>Тип ресурса "поставщики"
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
|number|строка|Номер поставщика.|
|displayName|строка|Отображаемое имя поставщика.|
|address|[Навигационная. Посталаддресс](../resources/dynamics-complextypes.md)|Адрес поставщика.|
|phoneNumber|строка|Номер телефона поставщика.|
|email|строка|Адрес электронной почты поставщика.|
|веб-сайт|строка|Адрес веб-сайта поставщика.|
|Таксрегистратионнумбер|строка|Регистрационный номер налогоплательщика поставщика.|
|Курренциид|GUID|Идентификатор кода валюты по умолчанию для поставщика.|
|Курренцикоде|строка|Код валюты по умолчанию для поставщика.|
|irs1099Code|строка|Указывает код 1099 для поставщика. Только для США.|
|Пайменттермсид|GUID|КОД условий оплаты для поставщика по умолчанию.|
|Пайментмесодид|GUID|Идентификатор метода оплаты по умолчанию для поставщика.|
|Такслиабле|boolean|Указывает, является ли поставщик подлежащей налогообложению.|
|заблокировано|строка|Указывает, какие транзакции у поставщика, который не может быть разнесен. Допустимые значения: пусто, оплата или все|
|равномерно|числе|Сальдо поставщика. Только для чтения.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения поставщика. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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

