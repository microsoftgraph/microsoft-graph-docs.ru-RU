---
title: Список Усеркредентиалусажедетаилс
description: Получение списка объектов Усеркредентиалусажедетаилс для определенного клиента.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 1ea46387a4d4f4c0920a94a2d082a20090fe0bb0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871237"
---
# <a name="list-usercredentialusagedetails"></a>Список Усеркредентиалусажедетаилс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) для определенного клиента. Сведения включают сведения о пользователе, состояние сброса и причину сбоя.

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
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта функция поддерживает необязательный параметр запроса OData **$Filter**. **$Filter** можно применить к одному или нескольким из следующих свойств ресурса [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) .

| Свойства | Описание и пример |
|:--------- |:----------- |
| состав | Фильтрация по типу требуемых данных (регистрация VS Reset). Пример: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`. Поддерживаемые операторы фильтра:`eq` |
| userDisplayName | Фильтрация по отображаемому имени пользователя. Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`. Поддерживаемые операторы фильтра: `eq` и `startswith()`. Поддерживает не зависящий от регистра. |
| userPrincipalName  | Фильтрация по имени участника пользователя. Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.    Поддерживаемые операторы фильтра: `eq` и `startswith()`. Поддерживает не зависящий от регистра. |
| Выполнение | Фильтрация по состоянию действия. Пример: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`. Поддерживаемые операторы фильтра: `eq` и `orderby`. |
| Аусмесод  | Фильтрация по методам проверки подлинности, используемым во время регистрации. Пример: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`. Поддерживаемые операторы фильтра: `eq`. |
| failureReason | Фильтрация по причине сбоя (если действие завершилось с ошибкой). Пример: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`. Поддерживаемые операторы фильтра: `eq` и `startswith()`. Поддерживает не зависящий от регистра. |


## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) в тексте отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Все свойства возвращаются при фактическом вызове.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 258

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
