---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: efab6a02f4e5eba8081c5d5e2e17e748e1a55bd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518240"
---
# <a name="update-contactfolder"></a><span data-ttu-id="e710f-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="e710f-103">Update contactfolder</span></span>

<span data-ttu-id="e710f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e710f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e710f-105">Обновление свойств объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="e710f-105">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e710f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e710f-106">Permissions</span></span>
<span data-ttu-id="e710f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e710f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e710f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e710f-109">Permission type</span></span>      | <span data-ttu-id="e710f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e710f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e710f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e710f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e710f-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e710f-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e710f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e710f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e710f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e710f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e710f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e710f-115">Application</span></span> | <span data-ttu-id="e710f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e710f-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e710f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e710f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e710f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e710f-118">Request headers</span></span>
| <span data-ttu-id="e710f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e710f-119">Header</span></span>       | <span data-ttu-id="e710f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e710f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e710f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e710f-121">Authorization</span></span>  | <span data-ttu-id="e710f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e710f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e710f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e710f-124">Content-Type</span></span>  | <span data-ttu-id="e710f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e710f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e710f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e710f-127">Request body</span></span>
<span data-ttu-id="e710f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e710f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e710f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e710f-131">Property</span></span>     | <span data-ttu-id="e710f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e710f-132">Type</span></span>   |<span data-ttu-id="e710f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e710f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e710f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e710f-134">displayName</span></span>|<span data-ttu-id="e710f-135">String</span><span class="sxs-lookup"><span data-stu-id="e710f-135">String</span></span>|<span data-ttu-id="e710f-136">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="e710f-136">The folder's display name.</span></span>|
|<span data-ttu-id="e710f-137">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e710f-137">parentFolderId</span></span>|<span data-ttu-id="e710f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="e710f-138">String</span></span>|<span data-ttu-id="e710f-139">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="e710f-139">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e710f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e710f-140">Response</span></span>

<span data-ttu-id="e710f-141">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e710f-141">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e710f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="e710f-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e710f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e710f-143">Request</span></span>
<span data-ttu-id="e710f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e710f-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e710f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e710f-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e710f-146">C#</span><span class="sxs-lookup"><span data-stu-id="e710f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e710f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e710f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e710f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e710f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e710f-149">Java</span><span class="sxs-lookup"><span data-stu-id="e710f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e710f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e710f-150">Response</span></span>
<span data-ttu-id="e710f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e710f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
