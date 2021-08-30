---
title: Удаление удостоверения участника
description: Удалите члена из externalGroup, удалив соответствующий ресурс удостоверений.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a518b782b5b705759659cd20480f91217b4abea8
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697601"
---
# <a name="delete-identity"></a>Удаление удостоверений
Пространство имен: microsoft.graph.externalConnectors

Удалите [ресурс удостоверений,](../resources/externalconnectors-identity.md) чтобы удалить соответствующий член из [externalGroup.](../resources/externalconnectors-externalgroup.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All                 |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionId}/groups/{externalGroupId}/members/{identityId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "delete_identity"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
