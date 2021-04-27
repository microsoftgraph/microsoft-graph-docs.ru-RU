---
title: Обновление approvalStep
description: Применить утверждение или отказ в принятии решения по объекту approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0fe071b58709a7816a4ffd9c82627542c1905243
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048045"
---
# <a name="update-approvalstep"></a>Обновление approvalStep

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Применить утверждение или отказ в принятии решения по [объекту approvalStep.](../resources/approvalStep.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В следующей таблице показаны свойства, необходимые для этого метода.

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| reviewResult | String | Решение утвержденного. Возможные значения: `Approve`, `Deny`.|
| обоснование | String | Обоснование, связанное с решением утвержденного. |


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `204 No Content` ответа в тексте ответа. Однако если у вызываемого не имеется нужных разрешений, метод возвращает код ответа или если код утверждения не найден, метод `403 Forbidden` `404 Not found` возвращается . Если запрос уже утвержден другим утверждением на том же этапе утверждения, метод возвращается `409 Conflict` в органе ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstep-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-Type: application/json
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
