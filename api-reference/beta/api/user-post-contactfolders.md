---
title: Создание объекта ContactFolder
description: Создание объекта contactFolder в стандартной папке контактов пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9eb5f7066c190adbb6786e5d44e15763703fa204
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053351"
---
# <a name="create-contactfolder"></a><span data-ttu-id="883e9-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="883e9-103">Create ContactFolder</span></span>

<span data-ttu-id="883e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="883e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="883e9-105">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="883e9-105">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="883e9-106">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="883e9-106">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="883e9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="883e9-107">Permissions</span></span>
<span data-ttu-id="883e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="883e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="883e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="883e9-110">Permission type</span></span>      | <span data-ttu-id="883e9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="883e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="883e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="883e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="883e9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="883e9-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="883e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="883e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="883e9-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="883e9-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="883e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="883e9-116">Application</span></span> | <span data-ttu-id="883e9-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="883e9-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="883e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="883e9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="883e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="883e9-119">Request headers</span></span>
| <span data-ttu-id="883e9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="883e9-120">Header</span></span>       | <span data-ttu-id="883e9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="883e9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="883e9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="883e9-122">Authorization</span></span>  | <span data-ttu-id="883e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="883e9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="883e9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="883e9-125">Content-Type</span></span>  | <span data-ttu-id="883e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="883e9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="883e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="883e9-127">Request body</span></span>
<span data-ttu-id="883e9-128">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="883e9-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="883e9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="883e9-129">Response</span></span>

<span data-ttu-id="883e9-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="883e9-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="883e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="883e9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="883e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="883e9-132">Request</span></span>
<span data-ttu-id="883e9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="883e9-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="883e9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="883e9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts"
}
```
# <a name="c"></a>[<span data-ttu-id="883e9-135">C#</span><span class="sxs-lookup"><span data-stu-id="883e9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="883e9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="883e9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="883e9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="883e9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="883e9-138">Java</span><span class="sxs-lookup"><span data-stu-id="883e9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contactfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="883e9-139">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="883e9-139">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="883e9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="883e9-140">Response</span></span>
<span data-ttu-id="883e9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="883e9-141">Here is an example of the response.</span></span> <span data-ttu-id="883e9-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="883e9-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
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


