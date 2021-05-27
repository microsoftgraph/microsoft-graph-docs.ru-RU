---
title: 'accessPackageAssignmentRequest: отмена'
description: Отмена объектов accessPackageAssignmentRequest, которые находятся в состоянии отменяемого.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 281eebc1008f8c1c791ac6cc2694a458c86f526b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679668"
---
# <a name="accesspackageassignmentrequest-cancel"></a>accessPackageAssignmentRequest: отмена
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)отменяйте [объекты accessPackageAssignmentRequest,](../resources/accesspackageassignmentrequest.md) которые находятся в отменяемом состоянии: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Чтобы пользователь, не управляющий, отменил свой собственный запрос, запрос должен содержать **id** [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) и **запросStatus** со значением `cancelled` .

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK`.  Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel

{
  "id":"request-id",
  "requestStatus":"cancelled"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

