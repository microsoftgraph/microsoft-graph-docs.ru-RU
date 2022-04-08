---
title: Удаление delegatedAdminAccessAssignment
description: Удаление объекта delegatedAdminAccessAssignment.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 2f9342324f44e2abf63062f0252d50c27aa293ec
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704263"
---
# <a name="delete-delegatedadminaccessassignment"></a>Удаление delegatedAdminAccessAssignment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление объекта [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| DelegatedAdminRelationship.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/accessAssignments/{delegatedAdminAccessAssignmentId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|If-Match|If-match: {etag}. Последнее известное значение ETag для **удаляемого объекта delegatedAdminAccessAssignment** . Обязательный. Получение значения ETag из операции LIST или GET.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "delete_delegatedadminaccessassignment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments/a9d6cf90-083a-47dc-ace2-1da98be3f344
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

