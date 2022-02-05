---
title: 'accessPackageAssignmentRequest: reprocess'
description: Reprocess accessPackageAssignmentRequest objects.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
---

# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest: reprocess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](../resources/entitlementmanagement-overview.md) звонители могут автоматически повторить запрос пользователя на доступ к пакету доступа. Выполняется на [объекте accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) , запрос **которого** находится в состоянии или `DeliveryFailed` состоянии `PartiallyDelivered` . 

## <a name="permissions"></a>Разрешения:

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | EntitlementManagement.ReadWrite.All |
  
## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/reprocess
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код  `202 Accepted` ответа и возвращает запрос. Если объекта [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) не существует, `404 Not Found` этот метод возвращается или если код не действителен, `400 Bad Request` этот метод возвращает код ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted  
```
