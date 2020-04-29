---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 41ce52fb4de9348b8bec9ea2e99848ee230cb268
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511021"
---
# <a name="update-photo"></a><span data-ttu-id="609df-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="609df-103">Update photo</span></span>

<span data-ttu-id="609df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="609df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="609df-105">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="609df-105">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="609df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="609df-106">Permissions</span></span>
<span data-ttu-id="609df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="609df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="609df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="609df-109">Permission type</span></span>      | <span data-ttu-id="609df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="609df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="609df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="609df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="609df-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="609df-112">Not supported.</span></span>    |
|<span data-ttu-id="609df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="609df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="609df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="609df-114">Not supported.</span></span>    |
|<span data-ttu-id="609df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="609df-115">Application</span></span> | <span data-ttu-id="609df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="609df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="609df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="609df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="609df-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="609df-118">Request headers</span></span>
| <span data-ttu-id="609df-119">Имя</span><span class="sxs-lookup"><span data-stu-id="609df-119">Name</span></span>       | <span data-ttu-id="609df-120">Тип</span><span class="sxs-lookup"><span data-stu-id="609df-120">Type</span></span> | <span data-ttu-id="609df-121">Описание</span><span class="sxs-lookup"><span data-stu-id="609df-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="609df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="609df-122">Authorization</span></span>  | <span data-ttu-id="609df-123">string</span><span class="sxs-lookup"><span data-stu-id="609df-123">string</span></span>  | <span data-ttu-id="609df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="609df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="609df-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="609df-126">Request body</span></span>
<span data-ttu-id="609df-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="609df-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="609df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="609df-130">Property</span></span>     | <span data-ttu-id="609df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="609df-131">Type</span></span>   |<span data-ttu-id="609df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="609df-132">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="609df-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="609df-133">Response</span></span>

<span data-ttu-id="609df-134">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="609df-134">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="609df-135">Пример</span><span class="sxs-lookup"><span data-stu-id="609df-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="609df-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="609df-136">Request</span></span>
<span data-ttu-id="609df-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="609df-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="609df-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="609df-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
# <a name="c"></a>[<span data-ttu-id="609df-139">C#</span><span class="sxs-lookup"><span data-stu-id="609df-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="609df-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="609df-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="609df-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="609df-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="609df-142">Java</span><span class="sxs-lookup"><span data-stu-id="609df-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="609df-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="609df-143">Response</span></span>
<span data-ttu-id="609df-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="609df-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
