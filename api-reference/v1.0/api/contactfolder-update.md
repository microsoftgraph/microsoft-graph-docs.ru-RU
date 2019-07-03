---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6ac7d76e912034cc90772558d6d632212ce0b0eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442974"
---
# <a name="update-contactfolder"></a><span data-ttu-id="c505b-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="c505b-103">Update contactfolder</span></span>

<span data-ttu-id="c505b-104">Обновление свойств объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c505b-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c505b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c505b-105">Permissions</span></span>
<span data-ttu-id="c505b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c505b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c505b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c505b-108">Permission type</span></span>      | <span data-ttu-id="c505b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c505b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c505b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c505b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c505b-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c505b-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c505b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c505b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c505b-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c505b-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c505b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c505b-114">Application</span></span> | <span data-ttu-id="c505b-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c505b-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c505b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c505b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c505b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c505b-117">Request headers</span></span>
| <span data-ttu-id="c505b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c505b-118">Header</span></span>       | <span data-ttu-id="c505b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c505b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c505b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c505b-120">Authorization</span></span>  | <span data-ttu-id="c505b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c505b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c505b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c505b-123">Content-Type</span></span>  | <span data-ttu-id="c505b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c505b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c505b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c505b-126">Request body</span></span>
<span data-ttu-id="c505b-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c505b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c505b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c505b-130">Property</span></span>     | <span data-ttu-id="c505b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c505b-131">Type</span></span>   |<span data-ttu-id="c505b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c505b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c505b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c505b-133">displayName</span></span>|<span data-ttu-id="c505b-134">String</span><span class="sxs-lookup"><span data-stu-id="c505b-134">String</span></span>|<span data-ttu-id="c505b-135">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="c505b-135">The folder's display name.</span></span>|
|<span data-ttu-id="c505b-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c505b-136">parentFolderId</span></span>|<span data-ttu-id="c505b-137">String</span><span class="sxs-lookup"><span data-stu-id="c505b-137">String</span></span>|<span data-ttu-id="c505b-138">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="c505b-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="c505b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c505b-139">Response</span></span>

<span data-ttu-id="c505b-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c505b-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c505b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c505b-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c505b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c505b-142">Request</span></span>
<span data-ttu-id="c505b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c505b-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c505b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c505b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c505b-145">C#</span><span class="sxs-lookup"><span data-stu-id="c505b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c505b-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="c505b-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c505b-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c505b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c505b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c505b-148">Response</span></span>
<span data-ttu-id="c505b-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c505b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
