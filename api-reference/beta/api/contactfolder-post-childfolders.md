---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7f782f32bd08532cad2efb10a101e3f96230bdbe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436876"
---
# <a name="create-contactfolder"></a><span data-ttu-id="21df8-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="21df8-103">Create ContactFolder</span></span>

<span data-ttu-id="21df8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21df8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21df8-105">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="21df8-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="21df8-106">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="21df8-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="21df8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21df8-107">Permissions</span></span>
<span data-ttu-id="21df8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21df8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21df8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21df8-110">Permission type</span></span>      | <span data-ttu-id="21df8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21df8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21df8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21df8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21df8-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21df8-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="21df8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21df8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21df8-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21df8-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="21df8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21df8-116">Application</span></span> | <span data-ttu-id="21df8-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21df8-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="21df8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21df8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="21df8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21df8-119">Request headers</span></span>
| <span data-ttu-id="21df8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21df8-120">Header</span></span>       | <span data-ttu-id="21df8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="21df8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21df8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21df8-122">Authorization</span></span>  | <span data-ttu-id="21df8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21df8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="21df8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21df8-125">Content-Type</span></span>  | <span data-ttu-id="21df8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21df8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21df8-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="21df8-128">Request body</span></span>
<span data-ttu-id="21df8-129">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21df8-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="21df8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="21df8-130">Response</span></span>

<span data-ttu-id="21df8-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21df8-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21df8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="21df8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21df8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="21df8-133">Request</span></span>
<span data-ttu-id="21df8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21df8-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21df8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="21df8-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="21df8-136">C#</span><span class="sxs-lookup"><span data-stu-id="21df8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21df8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21df8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21df8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21df8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="21df8-139">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21df8-139">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="21df8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="21df8-140">Response</span></span>
<span data-ttu-id="21df8-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21df8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
