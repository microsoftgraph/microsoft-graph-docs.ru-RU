---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 05a42bfb00cb56cd560151976bc8b7c7d6ed59ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081778"
---
# <a name="companyinformation-resource-type"></a>Тип ресурса Компанинформатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения, указанные для текущей компании в Dynamics 365 Business Central, такие как имя, адрес, адрес электронной почты и адрес веб-сайта.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Компанинформатион](../api/dynamics-companyinformation-get.md)|компанинформатион|Получает сведения о компании.|
|[Исправление Компанинформатион](../api/dynamics-companyinformation-update.md)|компанинформатион|Обновляет сведения о компании.|


## <a name="properties"></a>Свойства
| Свойство     | Тип      |Описание                           |
|:-------------|:--------|:-------------------------------------|
|id            |GUID|Уникальный идентификатор компании. Не редактируемые.|
|displayName   |string   |Отображаемое имя компании.           |
|address       |[Навигационная. посталаддресс](../resources/dynamics-complextypes.md)|Адрес компании. Просмотрите сложный тип для получения дополнительных сведений.|
|phoneNumber   |string   |Номер телефона компании.       |
|faxNumber     |string   |Номер факса компании.             |
|email         |строка   |Адрес электронной почты компании.          |
|веб-сайт       |string   |Адрес веб-сайта компании.        |
|таксрегистратионнумбер|string|Регистрационный номер налогоплательщика компании.|
|курренцикоде  |string   |Валюта, в которой компания выполняет бизнес. Только для чтения.|
|куррентфискалеарстартдате|date|Текущая дата начала финансового года компании. Только для чтения.|
|источников      |string   |Отрасль, в которой участвует компания.  |
|графические       |stream   |Логотип компании. Только для чтения.          |
|бусинесспрофилеид|string|Идентификатор бизнес-профиля, связанный с компанией "Финансы". Только для чтения.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения компании. Только для чтения.|  


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено представление объекта Компанинформатион в формате JSON.
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```



