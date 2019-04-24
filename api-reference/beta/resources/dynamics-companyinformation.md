---
title: Тип ресурса Компанинформатион
description: Сведения о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507275"
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
|phoneNumber   |строка   |Номер телефона компании.       |
|faxNumber     |строка   |Номер факса компании.             |
|email         |строка   |Адрес электронной почты компании.          |
|веб-сайт       |строка   |Адрес веб-сайта компании.        |
|Таксрегистратионнумбер|строка|Регистрационный номер налогоплательщика компании.|
|Курренцикоде  |строка   |Валюта, в которой компания выполняет бизнес. Только для чтения.|
|Куррентфискалеарстартдате|дата|Текущая дата начала финансового года компании. Только для чтения.|
|источников      |строка   |Отрасль, в которой участвует компания.  |
|графические       |stream   |Логотип компании. Только для чтения.          |
|Бусинесспрофилеид|строка|Идентификатор бизнес-профиля, связанный с компанией "Финансы". Только для чтения.|
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

