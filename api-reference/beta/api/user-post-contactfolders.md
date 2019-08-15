---
title: Создание объекта ContactFolder
description: Создание объекта contactFolder в стандартной папке контактов пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ed499640f12894dc19c8da7122804134b9b9781
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421948"
---
# <a name="create-contactfolder"></a><span data-ttu-id="52a40-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="52a40-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a40-104">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="52a40-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="52a40-105">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="52a40-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="52a40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52a40-106">Permissions</span></span>
<span data-ttu-id="52a40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52a40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52a40-109">Permission type</span></span>      | <span data-ttu-id="52a40-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52a40-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52a40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52a40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52a40-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52a40-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="52a40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52a40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52a40-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52a40-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="52a40-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52a40-115">Application</span></span> | <span data-ttu-id="52a40-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52a40-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52a40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52a40-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="52a40-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52a40-118">Request headers</span></span>
| <span data-ttu-id="52a40-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52a40-119">Header</span></span>       | <span data-ttu-id="52a40-120">Значение</span><span class="sxs-lookup"><span data-stu-id="52a40-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="52a40-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52a40-121">Authorization</span></span>  | <span data-ttu-id="52a40-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52a40-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="52a40-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52a40-124">Content-Type</span></span>  | <span data-ttu-id="52a40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52a40-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="52a40-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52a40-126">Request body</span></span>
<span data-ttu-id="52a40-127">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52a40-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="52a40-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="52a40-128">Response</span></span>

<span data-ttu-id="52a40-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52a40-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52a40-130">Пример</span><span class="sxs-lookup"><span data-stu-id="52a40-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52a40-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="52a40-131">Request</span></span>
<span data-ttu-id="52a40-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52a40-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52a40-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="52a40-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52a40-134">C#</span><span class="sxs-lookup"><span data-stu-id="52a40-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52a40-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52a40-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52a40-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="52a40-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="52a40-137">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52a40-137">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="52a40-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="52a40-138">Response</span></span>
<span data-ttu-id="52a40-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52a40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
