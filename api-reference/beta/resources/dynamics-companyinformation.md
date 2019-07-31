---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2e23660775ba96b3f898840b0bad2b53eff9584a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012670"
---
# <a name="companyinformation-resource-type"></a>Тип ресурса Компанинформатион
Представляет сведения, указанные для текущей компании в Dynamics 365 Business Central, такие как имя, адрес, адрес электронной почты и адрес веб-сайта.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Компанинформатион](../api/dynamics-companyinformation-get.md)|Компанинформатион|Получает сведения о компании.|
|[Исправление Компанинформатион](../api/dynamics-companyinformation-update.md)|Компанинформатион|Обновляет сведения о компании.|


## <a name="properties"></a>Свойства
| Свойство     | Тип      |Описание                           |
|:-------------|:--------|:-------------------------------------|
|id            |GUID|Уникальный идентификатор компании. Не редактируемые.|
|displayName   |string   |Отображаемое имя компании.           |
|address       |[Навигационная. Посталаддресс](../resources/dynamics-complextypes.md)|Адрес компании. Просмотрите сложный тип для получения дополнительных сведений.|
|phoneNumber   |string   |Номер телефона компании.       |
|faxNumber     |string   |Номер факса компании.             |
|email         |string   |Адрес электронной почты компании.          |
|веб-сайт       |string   |Адрес веб-сайта компании.        |
|Таксрегистратионнумбер|string|Регистрационный номер налогоплательщика компании.|
|Курренцикоде  |string   |Валюта, в которой компания выполняет бизнес. Только для чтения.|
|Куррентфискалеарстартдате|date|Текущая дата начала финансового года компании. Только для чтения.|
|источников      |string   |Отрасль, в которой участвует компания.  |
|графические       |stream   |Логотип компании. Только для чтения.          |
|Бусинесспрофилеид|string|Идентификатор бизнес-профиля, связанный с компанией "Финансы". Только для чтения.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения компании. Только для чтения.|  


## <a name="relationships"></a>Отношения
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

