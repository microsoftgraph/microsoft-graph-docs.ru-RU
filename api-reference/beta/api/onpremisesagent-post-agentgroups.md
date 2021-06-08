---
title: Назначение onPremisesAgent onPremisesAgentGroup
description: Назначение onPremisesAgent для onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9788e4485ba5c81453aac5087661bf3ea3e98299
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787550"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a>Назначение onPremisesAgent onPremisesAgentGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Назначьте onPremisesAgent](../resources/onpremisesagent.md) [объекту onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:--------------------------------------|:---------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Тело запроса

В теле запроса предоставляем JSON-представление ссылки OData на объект [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и новый объект `201 Created` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В теле запроса предоставляем JSON-представление ссылки OData на [объект onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



