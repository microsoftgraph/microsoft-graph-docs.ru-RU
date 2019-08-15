---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 48c5a617b2f13fd5f9267b848336930709102996
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417948"
---
# <a name="create-contactfolder"></a><span data-ttu-id="522b0-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="522b0-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="522b0-104">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="522b0-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="522b0-105">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="522b0-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="522b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="522b0-106">Permissions</span></span>
<span data-ttu-id="522b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="522b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="522b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="522b0-109">Permission type</span></span>      | <span data-ttu-id="522b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="522b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="522b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="522b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="522b0-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="522b0-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="522b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="522b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="522b0-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="522b0-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="522b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="522b0-115">Application</span></span> | <span data-ttu-id="522b0-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="522b0-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="522b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="522b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="522b0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="522b0-118">Request headers</span></span>
| <span data-ttu-id="522b0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="522b0-119">Header</span></span>       | <span data-ttu-id="522b0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="522b0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="522b0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="522b0-121">Authorization</span></span>  | <span data-ttu-id="522b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="522b0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="522b0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="522b0-124">Content-Type</span></span>  | <span data-ttu-id="522b0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="522b0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="522b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="522b0-127">Request body</span></span>
<span data-ttu-id="522b0-128">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="522b0-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="522b0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="522b0-129">Response</span></span>

<span data-ttu-id="522b0-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="522b0-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="522b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="522b0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="522b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="522b0-132">Request</span></span>
<span data-ttu-id="522b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="522b0-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="522b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="522b0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="522b0-135">C#</span><span class="sxs-lookup"><span data-stu-id="522b0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="522b0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="522b0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="522b0-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="522b0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="522b0-138">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="522b0-138">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="522b0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="522b0-139">Response</span></span>
<span data-ttu-id="522b0-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="522b0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
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
