---
title: 'accessPackageAssignmentRequest: reprocess'
description: Reprocess accessPackageAssignmentRequest objects.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 39104bb29ba7b1f8a9e672775781a5303ab0fa81
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650743"
---
# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest: reprocess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](../resources/entitlementmanagement-overview.md)звонители могут автоматически повторить запрос пользователя на доступ к пакету доступа. Выполняется на [объекте accessPackageAssignmentRequest,](../resources/accesspackageassignmentrequest.md) запрос **которого** находится в состоянии или `DeliveryFailed` `PartiallyDelivered` состоянии. 

## <a name="permissions"></a>Разрешения

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
POST /identityGovernance/entitlementManagement/accessPackageAssignmentsRequests/{id}/reprocess  
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код  `202 Accepted` ответа и возвращает запрос. Если объекта [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) не существует, этот метод возвращается или если код не действителен, этот метод возвращает код `404 Not Found`  `400 Bad Request` ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentsrequest"
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
