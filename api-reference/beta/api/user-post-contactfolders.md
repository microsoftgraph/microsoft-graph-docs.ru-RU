---
title: Создание объекта ContactFolder
description: Создание объекта contactFolder в стандартной папке контактов пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1e1da488913703552394b7e2e761151933e10a99
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269533"
---
# <a name="create-contactfolder"></a><span data-ttu-id="d7186-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="d7186-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7186-104">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7186-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="d7186-105">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="d7186-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d7186-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7186-106">Permissions</span></span>
<span data-ttu-id="d7186-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7186-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7186-109">Permission type</span></span>      | <span data-ttu-id="d7186-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7186-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7186-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7186-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7186-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7186-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d7186-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7186-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7186-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7186-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d7186-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7186-115">Application</span></span> | <span data-ttu-id="d7186-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7186-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7186-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7186-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="d7186-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7186-118">Request headers</span></span>
| <span data-ttu-id="d7186-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7186-119">Header</span></span>       | <span data-ttu-id="d7186-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d7186-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7186-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7186-121">Authorization</span></span>  | <span data-ttu-id="d7186-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7186-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7186-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7186-124">Content-Type</span></span>  | <span data-ttu-id="d7186-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7186-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7186-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d7186-126">Request body</span></span>
<span data-ttu-id="d7186-127">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7186-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7186-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7186-128">Response</span></span>

<span data-ttu-id="d7186-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7186-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7186-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d7186-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7186-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7186-131">Request</span></span>
<span data-ttu-id="d7186-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7186-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="d7186-133">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7186-133">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d7186-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7186-134">Response</span></span>
<span data-ttu-id="d7186-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7186-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d7186-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d7186-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d7186-139">C#</span><span class="sxs-lookup"><span data-stu-id="d7186-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contactfolder_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7186-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="d7186-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contactfolder_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d7186-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d7186-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contactfolder_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
