---
title: Обновление oAuth2PermissionGrant
description: Обновление свойств объекта oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: b54254123b38865e16e9fb5780c06effd538a970
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878938"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="7aacd-103">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="7aacd-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aacd-104">Обновление свойств объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="7aacd-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aacd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aacd-105">Permissions</span></span>

<span data-ttu-id="7aacd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7aacd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aacd-108">Permission type</span></span>      | <span data-ttu-id="7aacd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aacd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aacd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aacd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aacd-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7aacd-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7aacd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aacd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aacd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aacd-113">Not supported.</span></span>    |
|<span data-ttu-id="7aacd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aacd-114">Application</span></span> | <span data-ttu-id="7aacd-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aacd-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aacd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aacd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7aacd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aacd-117">Request headers</span></span>
| <span data-ttu-id="7aacd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7aacd-118">Name</span></span>       | <span data-ttu-id="7aacd-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7aacd-119">Type</span></span> | <span data-ttu-id="7aacd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7aacd-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7aacd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aacd-121">Authorization</span></span>  | <span data-ttu-id="7aacd-122">string</span><span class="sxs-lookup"><span data-stu-id="7aacd-122">string</span></span>  | <span data-ttu-id="7aacd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aacd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aacd-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7aacd-125">Request body</span></span>
<span data-ttu-id="7aacd-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7aacd-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7aacd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7aacd-129">Property</span></span>     | <span data-ttu-id="7aacd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7aacd-130">Type</span></span>   |<span data-ttu-id="7aacd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7aacd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aacd-132">scope</span><span class="sxs-lookup"><span data-stu-id="7aacd-132">scope</span></span>|<span data-ttu-id="7aacd-133">String</span><span class="sxs-lookup"><span data-stu-id="7aacd-133">String</span></span>| <span data-ttu-id="7aacd-134">Указывает значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="7aacd-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="7aacd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aacd-135">Response</span></span>

<span data-ttu-id="7aacd-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7aacd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aacd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7aacd-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7aacd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aacd-139">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7aacd-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aacd-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7aacd-141">C#</span><span class="sxs-lookup"><span data-stu-id="7aacd-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aacd-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="7aacd-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7aacd-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7aacd-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7aacd-144">Java</span><span class="sxs-lookup"><span data-stu-id="7aacd-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7aacd-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aacd-145">Response</span></span>

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
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
