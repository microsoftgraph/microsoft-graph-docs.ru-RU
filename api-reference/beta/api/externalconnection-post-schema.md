---
title: Создание схемы
description: Создайте схему для подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7fd9a9caa8c85df45fb292f822a7a1959175316b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422147"
---
# <a name="create-schema"></a><span data-ttu-id="9b805-103">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="9b805-103">Create schema</span></span>

<span data-ttu-id="9b805-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9b805-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b805-105">Создайте схему для [подключения](../resources/externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="9b805-105">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

<span data-ttu-id="9b805-106">Поддерживаются два типа схемы: настраиваемые элементы и файлы.</span><span class="sxs-lookup"><span data-stu-id="9b805-106">Two schema types are supported: custom items, and files.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="9b805-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b805-107">Permissions</span></span>

<span data-ttu-id="9b805-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b805-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b805-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b805-110">Permission type</span></span>                        | <span data-ttu-id="9b805-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b805-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b805-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b805-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b805-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b805-113">Not supported.</span></span> |
| <span data-ttu-id="9b805-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b805-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b805-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b805-115">Not supported.</span></span> |
| <span data-ttu-id="9b805-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b805-116">Application</span></span>                            | <span data-ttu-id="9b805-117">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b805-117">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b805-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b805-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="9b805-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b805-119">Request headers</span></span>

| <span data-ttu-id="9b805-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9b805-120">Name</span></span>                  | <span data-ttu-id="9b805-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9b805-121">Description</span></span>                                          |
|:----------------------|:-----------------------------------------------------|
| <span data-ttu-id="9b805-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b805-122">Authorization</span></span>         | <span data-ttu-id="9b805-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b805-p102">Bearer {token}. Required.</span></span>                            |
| <span data-ttu-id="9b805-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b805-125">Content-Type</span></span>          | <span data-ttu-id="9b805-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b805-p103">application/json. Required.</span></span>                          |
| <span data-ttu-id="9b805-128">Предпочитать: ответ — Async</span><span class="sxs-lookup"><span data-stu-id="9b805-128">Prefer: respond-async</span></span> | <span data-ttu-id="9b805-129">Используйте этот параметр, чтобы запрос выполнялся асинхронно.</span><span class="sxs-lookup"><span data-stu-id="9b805-129">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="9b805-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9b805-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b805-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b805-131">Request body</span></span>

<span data-ttu-id="9b805-132">В тексте запроса добавьте представление объекта [схемы](../resources/schema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b805-132">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="9b805-133">При регистрации настраиваемой схемы `schema` элемента объекту должно быть присвоено `baseType` свойство, которое `microsoft.graph.externalItem` должно содержать `properties` свойство.</span><span class="sxs-lookup"><span data-stu-id="9b805-133">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="9b805-134">`properties` Объект должен содержать по крайней мере одно свойство (не более 64).</span><span class="sxs-lookup"><span data-stu-id="9b805-134">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

<span data-ttu-id="9b805-135">При регистрации схемы файла для `schema` `baseType` `microsoft.graph.externalFile`свойства объекта должно быть задано значение.</span><span class="sxs-lookup"><span data-stu-id="9b805-135">When registering a file schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalFile`.</span></span>

## <a name="response"></a><span data-ttu-id="9b805-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b805-136">Response</span></span>

<span data-ttu-id="9b805-137">Если `Prefer: respond-async` заголовок включен в запрос, в случае успешного выполнения этот метод возвращает код `202 Accepted` ОТКЛИКА и URL-адрес в `Location` заголовке ответа, который можно использовать для [получения состояния операции](../api/connectionoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="9b805-137">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="9b805-138">Без `Prefer: respond-async` заголовка, включенного в запрос (при успешном выполнении) Этот метод `201 Created` возвращает код отклика и новый объект [Schema](../resources/schema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b805-138">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="9b805-139">Создание схемы — длительный процесс, который может допустить превышение времени ожидания шлюза.</span><span class="sxs-lookup"><span data-stu-id="9b805-139">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="9b805-140">Рекомендуется использовать `Prefer: respond-async` заголовок, чтобы избежать ошибок времени ожидания.</span><span class="sxs-lookup"><span data-stu-id="9b805-140">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="9b805-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="9b805-141">Examples</span></span>

### <a name="example-1-register-custom-schema-asynchronously"></a><span data-ttu-id="9b805-142">Пример 1: асинхронная Регистрация настраиваемой схемы</span><span class="sxs-lookup"><span data-stu-id="9b805-142">Example 1: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="9b805-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b805-143">Request</span></span>

<span data-ttu-id="9b805-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b805-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b805-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b805-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "title",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9b805-146">C#</span><span class="sxs-lookup"><span data-stu-id="9b805-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b805-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b805-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b805-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b805-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="9b805-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b805-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9b805-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b805-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

### <a name="example-2-register-file-schema-synchronously"></a><span data-ttu-id="9b805-151">Пример 2: синхронная регистрация схемы файлов</span><span class="sxs-lookup"><span data-stu-id="9b805-151">Example 2: Register file schema synchronously</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="9b805-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b805-152">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9b805-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b805-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b805-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b805-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosofiles/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalFile"
}
```
# <a name="c"></a>[<span data-ttu-id="9b805-155">C#</span><span class="sxs-lookup"><span data-stu-id="9b805-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b805-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b805-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b805-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b805-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="9b805-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b805-158">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9b805-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9b805-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 201 Created

{
  "baseType": "microsoft.graph.externalFile"
}
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
