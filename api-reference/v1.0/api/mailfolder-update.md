---
title: Обновление объекта MailFolder
description: Обновление свойств объекта MailFolder.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3842eba43eee73c789669978d770075f4979158a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136139"
---
# <a name="update-mailfolder"></a><span data-ttu-id="f3c21-103">Обновление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="f3c21-103">Update mailfolder</span></span>

<span data-ttu-id="f3c21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3c21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3c21-105">Обновление свойств объекта MailFolder.</span><span class="sxs-lookup"><span data-stu-id="f3c21-105">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3c21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c21-106">Permissions</span></span>
<span data-ttu-id="f3c21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3c21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c21-109">Permission type</span></span>      | <span data-ttu-id="f3c21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3c21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3c21-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3c21-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f3c21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3c21-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3c21-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f3c21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c21-115">Application</span></span> | <span data-ttu-id="f3c21-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3c21-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3c21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f3c21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c21-118">Request headers</span></span>
| <span data-ttu-id="f3c21-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3c21-119">Header</span></span>       | <span data-ttu-id="f3c21-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f3c21-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3c21-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c21-121">Authorization</span></span>  | <span data-ttu-id="f3c21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c21-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f3c21-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3c21-124">Content-Type</span></span>  | <span data-ttu-id="f3c21-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c21-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3c21-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3c21-127">Request body</span></span>
<span data-ttu-id="f3c21-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f3c21-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f3c21-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3c21-131">Property</span></span>     | <span data-ttu-id="f3c21-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f3c21-132">Type</span></span>   |<span data-ttu-id="f3c21-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f3c21-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3c21-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f3c21-134">displayName</span></span>|<span data-ttu-id="f3c21-135">Строка</span><span class="sxs-lookup"><span data-stu-id="f3c21-135">String</span></span>|<span data-ttu-id="f3c21-136">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f3c21-136">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="f3c21-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c21-137">Response</span></span>

<span data-ttu-id="f3c21-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c21-138">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3c21-139">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c21-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3c21-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c21-140">Request</span></span>
<span data-ttu-id="f3c21-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c21-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3c21-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3c21-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="f3c21-143">C#</span><span class="sxs-lookup"><span data-stu-id="f3c21-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3c21-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3c21-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3c21-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3c21-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3c21-146">Java</span><span class="sxs-lookup"><span data-stu-id="f3c21-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f3c21-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c21-147">Response</span></span>
<span data-ttu-id="f3c21-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3c21-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

