---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b8a1e516d32af28c30be38117df78c6d7c040223
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507272"
---
# <a name="create-contactfolder"></a><span data-ttu-id="b6b08-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="b6b08-103">Create ContactFolder</span></span>

<span data-ttu-id="b6b08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6b08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6b08-105">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="b6b08-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="b6b08-106">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="b6b08-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b6b08-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6b08-107">Permissions</span></span>
<span data-ttu-id="b6b08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6b08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6b08-110">Permission type</span></span>      | <span data-ttu-id="b6b08-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6b08-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6b08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6b08-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6b08-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6b08-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b6b08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6b08-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6b08-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6b08-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b6b08-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6b08-116">Application</span></span> | <span data-ttu-id="b6b08-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6b08-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6b08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6b08-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="b6b08-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6b08-119">Request headers</span></span>
| <span data-ttu-id="b6b08-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6b08-120">Header</span></span>       | <span data-ttu-id="b6b08-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b6b08-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6b08-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6b08-122">Authorization</span></span>  | <span data-ttu-id="b6b08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6b08-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b6b08-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6b08-125">Content-Type</span></span>  | <span data-ttu-id="b6b08-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6b08-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6b08-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6b08-128">Request body</span></span>
<span data-ttu-id="b6b08-129">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6b08-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6b08-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b08-130">Response</span></span>

<span data-ttu-id="b6b08-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b08-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6b08-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b6b08-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6b08-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b08-133">Request</span></span>

<span data-ttu-id="b6b08-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b08-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6b08-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6b08-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json

{
  "displayName": "Family"
}
```
# <a name="c"></a>[<span data-ttu-id="b6b08-136">C#</span><span class="sxs-lookup"><span data-stu-id="b6b08-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6b08-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6b08-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6b08-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6b08-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6b08-139">Java</span><span class="sxs-lookup"><span data-stu-id="b6b08-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contactfolder-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b6b08-140">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6b08-140">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="b6b08-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b08-141">Response</span></span>

<span data-ttu-id="b6b08-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6b08-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Family",
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


