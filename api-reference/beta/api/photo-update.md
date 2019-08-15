---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 111521b59711815e3b447e296c3cfc425347cbd9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413639"
---
# <a name="update-photo"></a><span data-ttu-id="06ca8-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="06ca8-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06ca8-104">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="06ca8-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06ca8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06ca8-105">Permissions</span></span>
<span data-ttu-id="06ca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ca8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06ca8-108">Permission type</span></span>      | <span data-ttu-id="06ca8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06ca8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06ca8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06ca8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06ca8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06ca8-111">Not supported.</span></span>    |
|<span data-ttu-id="06ca8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06ca8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06ca8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06ca8-113">Not supported.</span></span>    |
|<span data-ttu-id="06ca8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06ca8-114">Application</span></span> | <span data-ttu-id="06ca8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06ca8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06ca8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06ca8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="06ca8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06ca8-117">Request headers</span></span>
| <span data-ttu-id="06ca8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="06ca8-118">Name</span></span>       | <span data-ttu-id="06ca8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="06ca8-119">Type</span></span> | <span data-ttu-id="06ca8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06ca8-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06ca8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06ca8-121">Authorization</span></span>  | <span data-ttu-id="06ca8-122">string</span><span class="sxs-lookup"><span data-stu-id="06ca8-122">string</span></span>  | <span data-ttu-id="06ca8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06ca8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06ca8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06ca8-125">Request body</span></span>
<span data-ttu-id="06ca8-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="06ca8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="06ca8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="06ca8-129">Property</span></span>     | <span data-ttu-id="06ca8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="06ca8-130">Type</span></span>   |<span data-ttu-id="06ca8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="06ca8-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="06ca8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="06ca8-132">Response</span></span>

<span data-ttu-id="06ca8-133">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06ca8-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06ca8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="06ca8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06ca8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="06ca8-135">Request</span></span>
<span data-ttu-id="06ca8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06ca8-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06ca8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="06ca8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06ca8-138">C#</span><span class="sxs-lookup"><span data-stu-id="06ca8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06ca8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06ca8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06ca8-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="06ca8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06ca8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="06ca8-141">Response</span></span>
<span data-ttu-id="06ca8-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06ca8-142">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
