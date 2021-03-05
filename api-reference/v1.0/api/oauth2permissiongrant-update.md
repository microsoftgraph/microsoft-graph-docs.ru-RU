---
title: Обновление oAuth2PermissionGrant
description: Обновление свойств oAuth2PermissionGrant, представляющего делегированную лицензию.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: fd75e020e69888c81cf4a9c53c180585ace73c7e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441776"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="1e531-103">Обновление делегированного разрешения (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="1e531-103">Update a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="1e531-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e531-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="1e531-105">Обновление свойств [объекта oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) представляющего делегированную выдачу разрешений.</span><span class="sxs-lookup"><span data-stu-id="1e531-105">Update the properties of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object, representing a delegated permission grant.</span></span>

<span data-ttu-id="1e531-106">**OAuth2PermissionGrant** можно обновить, чтобы изменить, какие делегированная разрешения предоставляется, путем добавления или удаления элементов из списка в **области**.</span><span class="sxs-lookup"><span data-stu-id="1e531-106">An **oAuth2PermissionGrant** can be updated to change which delegated permissions are granted, by adding or removing items from the list in **scopes**.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e531-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e531-107">Permissions</span></span>

<span data-ttu-id="1e531-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e531-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e531-110">Permission type</span></span>      | <span data-ttu-id="1e531-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e531-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e531-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e531-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e531-113">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e531-113">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e531-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e531-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e531-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e531-115">Not supported.</span></span>    |
|<span data-ttu-id="1e531-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e531-116">Application</span></span> | <span data-ttu-id="1e531-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e531-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e531-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e531-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e531-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e531-119">Request headers</span></span>

| <span data-ttu-id="1e531-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1e531-120">Name</span></span>       | <span data-ttu-id="1e531-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1e531-121">Type</span></span> | <span data-ttu-id="1e531-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1e531-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1e531-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e531-123">Authorization</span></span>  | <span data-ttu-id="1e531-124">string</span><span class="sxs-lookup"><span data-stu-id="1e531-124">string</span></span>  | <span data-ttu-id="1e531-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e531-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e531-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e531-127">Request body</span></span>

<span data-ttu-id="1e531-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1e531-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e531-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e531-131">Property</span></span>     | <span data-ttu-id="1e531-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1e531-132">Type</span></span>   |<span data-ttu-id="1e531-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1e531-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e531-134">scope</span><span class="sxs-lookup"><span data-stu-id="1e531-134">scope</span></span>|<span data-ttu-id="1e531-135">String</span><span class="sxs-lookup"><span data-stu-id="1e531-135">String</span></span>| <span data-ttu-id="1e531-136">Указывает значение утверждения области, которое приложение ресурсов должно ожидать в маркере доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="1e531-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="1e531-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e531-137">Response</span></span>

<span data-ttu-id="1e531-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1e531-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e531-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1e531-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e531-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e531-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1e531-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e531-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1e531-143">C#</span><span class="sxs-lookup"><span data-stu-id="1e531-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e531-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e531-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e531-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e531-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e531-146">Java</span><span class="sxs-lookup"><span data-stu-id="1e531-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e531-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e531-147">Response</span></span>

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

