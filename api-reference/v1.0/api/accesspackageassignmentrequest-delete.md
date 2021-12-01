---
title: Удаление accessPackageAssignmentRequest
description: Удаление accessPackageAssignmentRequest.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a694dbb46b43a7cfe437e9c078a8dc2175edf98b
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242800"
---
# <a name="delete-accesspackageassignmentrequest"></a>Удаление accessPackageAssignmentRequest

Пространство имен: microsoft.graph


Удаление [объекта accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Этот запрос можно сделать, чтобы удалить отклоненный или завершенный запрос.  Вы не можете удалить запрос на назначение пакета доступа, если у него есть **объекты accessPackageAssignment.**

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentrequest"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


