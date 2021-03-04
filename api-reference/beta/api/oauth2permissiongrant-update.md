---
title: Обновление oAuth2PermissionGrant
description: Обновление свойств oAuth2PermissionGrant, представляющего делегированную лицензию.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0c9d3f60eeff2edd01d6926fb2fed18a3e508db4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447942"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="2b7d7-103">Обновление делегированного разрешения (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="2b7d7-103">Update a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="2b7d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b7d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b7d7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b7d7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b7d7-106">Обновление свойств [объекта oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) представляющего делегированную выдачу разрешений.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-106">Update the properties of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object, representing a delegated permission grant.</span></span>

<span data-ttu-id="2b7d7-107">**OAuth2PermissionGrant** можно обновить, чтобы изменить, какие делегированная разрешения предоставляется, путем добавления или удаления элементов из списка в **области**.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-107">An **oAuth2PermissionGrant** can be updated to change which delegated permissions are granted, by adding or removing items from the list in **scopes**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b7d7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b7d7-108">Permissions</span></span>

<span data-ttu-id="2b7d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b7d7-111">Permission type</span></span>      | <span data-ttu-id="2b7d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b7d7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b7d7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2b7d7-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b7d7-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b7d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b7d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b7d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-116">Not supported.</span></span>    |
|<span data-ttu-id="2b7d7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b7d7-117">Application</span></span> | <span data-ttu-id="2b7d7-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7d7-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b7d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b7d7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b7d7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b7d7-120">Request headers</span></span>

| <span data-ttu-id="2b7d7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2b7d7-121">Name</span></span>       | <span data-ttu-id="2b7d7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7d7-122">Type</span></span> | <span data-ttu-id="2b7d7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7d7-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b7d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b7d7-124">Authorization</span></span>  | <span data-ttu-id="2b7d7-125">string</span><span class="sxs-lookup"><span data-stu-id="2b7d7-125">string</span></span>  | <span data-ttu-id="2b7d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b7d7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b7d7-128">Request body</span></span>

<span data-ttu-id="2b7d7-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2b7d7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b7d7-132">Property</span></span>     | <span data-ttu-id="2b7d7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7d7-133">Type</span></span>   |<span data-ttu-id="2b7d7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7d7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b7d7-135">scope</span><span class="sxs-lookup"><span data-stu-id="2b7d7-135">scope</span></span>|<span data-ttu-id="2b7d7-136">String</span><span class="sxs-lookup"><span data-stu-id="2b7d7-136">String</span></span>| <span data-ttu-id="2b7d7-137">Указывает значение утверждения области, которое приложение ресурсов должно ожидать в маркере доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-137">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="2b7d7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7d7-138">Response</span></span>

<span data-ttu-id="2b7d7-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2b7d7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b7d7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2b7d7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b7d7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b7d7-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2b7d7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7d7-143">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```

# <a name="c"></a>[<span data-ttu-id="2b7d7-144">C#</span><span class="sxs-lookup"><span data-stu-id="2b7d7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b7d7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b7d7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b7d7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b7d7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b7d7-147">Java</span><span class="sxs-lookup"><span data-stu-id="2b7d7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2b7d7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7d7-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


