---
title: Обновление oAuth2PermissionGrant
description: Обновление свойств объекта oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 056b1491de7044efac3a51612590766949fd7a96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456617"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="dd401-103">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="dd401-103">Update oAuth2PermissionGrant</span></span>

<span data-ttu-id="dd401-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd401-105">Обновление свойств объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="dd401-105">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd401-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd401-106">Permissions</span></span>

<span data-ttu-id="dd401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd401-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd401-109">Permission type</span></span>      | <span data-ttu-id="dd401-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd401-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd401-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd401-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd401-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd401-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd401-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd401-114">Not supported.</span></span>    |
|<span data-ttu-id="dd401-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd401-115">Application</span></span> | <span data-ttu-id="dd401-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd401-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd401-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd401-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd401-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd401-118">Request headers</span></span>
| <span data-ttu-id="dd401-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dd401-119">Name</span></span>       | <span data-ttu-id="dd401-120">Тип</span><span class="sxs-lookup"><span data-stu-id="dd401-120">Type</span></span> | <span data-ttu-id="dd401-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dd401-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd401-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd401-122">Authorization</span></span>  | <span data-ttu-id="dd401-123">string</span><span class="sxs-lookup"><span data-stu-id="dd401-123">string</span></span>  | <span data-ttu-id="dd401-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd401-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd401-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd401-126">Request body</span></span>
<span data-ttu-id="dd401-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dd401-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd401-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd401-130">Property</span></span>     | <span data-ttu-id="dd401-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd401-131">Type</span></span>   |<span data-ttu-id="dd401-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd401-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd401-133">scope</span><span class="sxs-lookup"><span data-stu-id="dd401-133">scope</span></span>|<span data-ttu-id="dd401-134">String</span><span class="sxs-lookup"><span data-stu-id="dd401-134">String</span></span>| <span data-ttu-id="dd401-135">Указывает значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="dd401-135">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="dd401-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd401-136">Response</span></span>

<span data-ttu-id="dd401-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dd401-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd401-139">Пример</span><span class="sxs-lookup"><span data-stu-id="dd401-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd401-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd401-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dd401-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd401-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dd401-142">C#</span><span class="sxs-lookup"><span data-stu-id="dd401-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd401-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd401-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd401-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd401-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd401-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd401-145">Response</span></span>

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
