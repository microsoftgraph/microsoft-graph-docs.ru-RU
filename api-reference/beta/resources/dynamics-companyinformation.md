---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ce982e7d03e4b2e5947381173d57706f6cf8f41e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505128"
---
# <a name="companyinformation-resource-type"></a>Тип ресурса Компанинформатион

Пространство имен: Microsoft. Graph

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
|phoneNumber   |строка   |Номер телефона компании.       |
|faxNumber     |строка   |Номер факса компании.             |
|email         |строка   |Адрес электронной почты компании.          |
|веб-сайт       |строка   |Адрес веб-сайта компании.        |
|таксрегистратионнумбер|строка|Регистрационный номер налогоплательщика компании.|
|курренцикоде  |строка   |Валюта, в которой компания выполняет бизнес. Только для чтения.|
|куррентфискалеарстартдате|date|Текущая дата начала финансового года компании. Только для чтения.|
|источников      |строка   |Отрасль, в которой участвует компания.  |
|графические       |stream   |Логотип компании. Только для чтения.          |
|бусинесспрофилеид|строка|Идентификатор бизнес-профиля, связанный с компанией "Финансы". Только для чтения.|
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

