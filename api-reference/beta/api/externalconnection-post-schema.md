---
title: Создание схемы
description: Создайте схему для подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 27820a392d0a37363f447609713f86df1affef15
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965594"
---
# <a name="create-schema"></a><span data-ttu-id="117ab-103">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="117ab-103">Create schema</span></span>

<span data-ttu-id="117ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="117ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="117ab-105">Создайте схему для [подключения](../resources/externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="117ab-105">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="117ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="117ab-106">Permissions</span></span>

<span data-ttu-id="117ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="117ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="117ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="117ab-109">Permission type</span></span>                        | <span data-ttu-id="117ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="117ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="117ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="117ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="117ab-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="117ab-112">Not supported.</span></span> |
| <span data-ttu-id="117ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="117ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="117ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="117ab-114">Not supported.</span></span> |
| <span data-ttu-id="117ab-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="117ab-115">Application</span></span>                            | <span data-ttu-id="117ab-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="117ab-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="117ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="117ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="117ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="117ab-118">Request headers</span></span>

| <span data-ttu-id="117ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="117ab-119">Name</span></span>                  | <span data-ttu-id="117ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="117ab-120">Description</span></span>                                                        |
|:----------------------|:-------------------------------------------------------------------|
| <span data-ttu-id="117ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="117ab-121">Authorization</span></span>         | <span data-ttu-id="117ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="117ab-p102">Bearer {token}. Required.</span></span>                                          |
| <span data-ttu-id="117ab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="117ab-124">Content-Type</span></span>          | <span data-ttu-id="117ab-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="117ab-p103">application/json. Required.</span></span>                                        |
| <span data-ttu-id="117ab-127">Предпочитать: ответ — Async</span><span class="sxs-lookup"><span data-stu-id="117ab-127">Prefer: respond-async</span></span> | <span data-ttu-id="117ab-128">Используйте этот параметр, чтобы запрос выполнялся асинхронно.</span><span class="sxs-lookup"><span data-stu-id="117ab-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="117ab-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="117ab-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="117ab-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="117ab-130">Request body</span></span>

<span data-ttu-id="117ab-131">В тексте запроса добавьте представление объекта [схемы](../resources/schema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="117ab-131">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="117ab-132">При регистрации настраиваемой схемы элемента `schema` объекту должно быть `baseType` присвоено свойство, которое `microsoft.graph.externalItem` должно содержать `properties` свойство.</span><span class="sxs-lookup"><span data-stu-id="117ab-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="117ab-133">`properties`Объект должен содержать по крайней мере одно свойство (не более 64).</span><span class="sxs-lookup"><span data-stu-id="117ab-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="117ab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="117ab-134">Response</span></span>

<span data-ttu-id="117ab-135">`Prefer: respond-async`Если заголовок включен в запрос, в случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и URL-адрес в `Location` заголовке ответа, который можно использовать для [получения состояния операции](../api/connectionoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="117ab-135">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="117ab-136">Без `Prefer: respond-async` заголовка, включенного в запрос (при успешном выполнении) Этот метод возвращает `201 Created` код отклика и новый объект [Schema](../resources/schema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="117ab-136">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="117ab-137">Создание схемы — длительный процесс, который может допустить превышение времени ожидания шлюза.</span><span class="sxs-lookup"><span data-stu-id="117ab-137">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="117ab-138">Рекомендуется использовать `Prefer: respond-async` заголовок, чтобы избежать ошибок времени ожидания.</span><span class="sxs-lookup"><span data-stu-id="117ab-138">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="117ab-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="117ab-139">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="117ab-140">Пример: асинхронная Регистрация настраиваемой схемы</span><span class="sxs-lookup"><span data-stu-id="117ab-140">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="117ab-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="117ab-141">Request</span></span>

<span data-ttu-id="117ab-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="117ab-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="117ab-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="117ab-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="117ab-144">C#</span><span class="sxs-lookup"><span data-stu-id="117ab-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="117ab-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="117ab-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="117ab-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="117ab-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="117ab-147">Java</span><span class="sxs-lookup"><span data-stu-id="117ab-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="117ab-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="117ab-148">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="117ab-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="117ab-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


