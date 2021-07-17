---
title: Создание схемы
description: Создайте схему для Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b89fdd9ec7785639526f02344c8b4c7bc43335b1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467696"
---
# <a name="create-schema"></a><span data-ttu-id="a065d-103">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="a065d-103">Create schema</span></span>

<span data-ttu-id="a065d-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="a065d-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a065d-105">Создайте схему подключения [Поиск (Майкрософт).](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="a065d-105">Create the schema for a Microsoft Search [connection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a065d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a065d-106">Permissions</span></span>

<span data-ttu-id="a065d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a065d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a065d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a065d-109">Permission type</span></span>                        | <span data-ttu-id="a065d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a065d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a065d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a065d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a065d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a065d-112">Not supported.</span></span> |
| <span data-ttu-id="a065d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a065d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a065d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a065d-114">Not supported.</span></span> |
| <span data-ttu-id="a065d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a065d-115">Application</span></span>                            | <span data-ttu-id="a065d-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a065d-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="a065d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a065d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="a065d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a065d-118">Request headers</span></span>

| <span data-ttu-id="a065d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a065d-119">Name</span></span>                  | <span data-ttu-id="a065d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a065d-120">Description</span></span>                                                        |
|:----------------------|:-------------------------------------------------------------------|
| <span data-ttu-id="a065d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a065d-121">Authorization</span></span>         | <span data-ttu-id="a065d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a065d-p102">Bearer {token}. Required.</span></span>                                          |
| <span data-ttu-id="a065d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a065d-124">Content-Type</span></span>          | <span data-ttu-id="a065d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a065d-p103">application/json. Required.</span></span>                                        |
| <span data-ttu-id="a065d-127">Предпочитаете: respond-async</span><span class="sxs-lookup"><span data-stu-id="a065d-127">Prefer: respond-async</span></span> | <span data-ttu-id="a065d-128">Используйте это, чтобы вызвать асинхронное выполнение запроса.</span><span class="sxs-lookup"><span data-stu-id="a065d-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="a065d-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a065d-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a065d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a065d-130">Request body</span></span>

<span data-ttu-id="a065d-131">В теле запроса поставляем представление JSON объекта [схемы.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="a065d-131">In the request body, supply a JSON representation of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

<span data-ttu-id="a065d-132">При регистрации настраиваемой схемы элементов объект должен иметь свойство, к котором должно быть установлено свойство, `schema` `baseType` и должен содержать `microsoft.graph.externalItem` `properties` его.</span><span class="sxs-lookup"><span data-stu-id="a065d-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="a065d-133">Объект должен содержать по крайней мере одно свойство, не `properties` более 64.</span><span class="sxs-lookup"><span data-stu-id="a065d-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="a065d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a065d-134">Response</span></span>

<span data-ttu-id="a065d-135">Если заготка включена в запрос, этот метод возвращает код ответа и URL-адрес в загонах ответа, которые можно использовать для получения состояния `Prefer: respond-async` `202 Accepted` `Location` [операции.](../api/externalconnectors-connectionoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="a065d-135">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/externalconnectors-connectionoperation-get.md).</span></span>

<span data-ttu-id="a065d-136">Без заголовка, включенного в запрос, в случае успешного использования этот метод возвращает код ответа и новый объект схемы в `Prefer: respond-async` `201 Created` тексте ответа. [](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="a065d-136">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="a065d-137">Создание схемы — это длительный процесс, склонный к выходу времени шлюза.</span><span class="sxs-lookup"><span data-stu-id="a065d-137">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="a065d-138">Рекомендуется использовать `Prefer: respond-async` заготку, чтобы избежать ошибок в периодике.</span><span class="sxs-lookup"><span data-stu-id="a065d-138">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="a065d-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="a065d-139">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="a065d-140">Пример. Регистрация настраиваемой схемы асинхронно</span><span class="sxs-lookup"><span data-stu-id="a065d-140">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="a065d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a065d-141">Request</span></span>

<span data-ttu-id="a065d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a065d-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a065d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a065d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
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
      "type": "string",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "string",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "string",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a065d-144">C#</span><span class="sxs-lookup"><span data-stu-id="a065d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a065d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a065d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a065d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a065d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a065d-147">Java</span><span class="sxs-lookup"><span data-stu-id="a065d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="a065d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a065d-148">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="a065d-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a065d-149">The following is an example of the response.</span></span>

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
