---
title: 'Reportroot.: Жеткредентиалусажесуммари'
description: Сообщите о текущем состоянии того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 6ec8afa24f83e50d2fcf354b37e1f5524eea2295
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488409"
---
# <a name="reportroot-getcredentialusagesummary"></a>Reportroot.: Жеткредентиалусажесуммари

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сообщите о текущем состоянии того, сколько пользователей в вашей организации использовало возможности самостоятельного сброса пароля.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Reports.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a>Параметры функции

Для настройки отклика можно использовать следующий параметр функции.

| Параметр | Тип | Описание |
|:--------- |:---- |:----------- |
| period | String | Задает период времени, для которого требуются данные об использовании. Пример: `/reports/getCredentialUsageSummary(period='D30')`. Поддерживаемые периоды: `D1`, `D7`, и `D30`. В периоде регистр не учитывается. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта функция поддерживает необязательный параметр запроса OData **$Filter**. **$Filter** можно применить к одному или нескольким из следующих свойств ресурса [кредентиалусажесуммари](../resources/credentialusagesummary.md) .

| Свойства | Описание и пример |
|:---- |:----------- |
| состав | Задает тип данных об использовании (регистрация и сброс). Пример: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`. Поддерживаемые операторы фильтра: `eq`. |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [кредентиалусажесуммари](../resources/credentialusagesummary.md) в тексте отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Все свойства возвращаются при фактическом вызове.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->