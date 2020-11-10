---
title: Создание Пермиссионгранткондитионсет в коллекции включенных элементов Пермиссионгрантполици
description: Добавьте условия, при которых событие предоставления разрешений включается в политику предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: a90c126f4a1d6de42bdd375f8fbb27e94688f711
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962801"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a>Создание Пермиссионгранткондитионсет в коллекции включенных элементов Пермиссионгрантполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте условия, при которых событие предоставления разрешений *включается* в политику предоставления разрешений. Это можно сделать, добавив [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в коллекцию **includes** объекта  [пермиссионгрантполици](../resources/permissionGrantPolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Policy.ReadWrite.PermissionGrant |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | Policy.ReadWrite.PermissionGrant |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В этом примере *все* делегированные разрешения для клиентских приложений из проверенных издателей включены в политику предоставления разрешений. Так как все остальные условия из [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) опущены, они будут принимать значения по умолчанию, которые в каждом случае являются самыми-инклюзивными.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-create-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
