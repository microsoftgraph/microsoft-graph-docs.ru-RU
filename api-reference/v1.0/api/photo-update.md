---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: 00d8f63509635c4f4aabe0deb02a59efa8af0f3c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856876"
---
# <a name="update-photo"></a><span data-ttu-id="3e1c3-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="3e1c3-103">Update photo</span></span>

<span data-ttu-id="3e1c3-104">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e1c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1c3-105">Permissions</span></span>
<span data-ttu-id="3e1c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e1c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e1c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1c3-108">Permission type</span></span>      | <span data-ttu-id="3e1c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e1c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e1c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e1c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e1c3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-111">Not supported.</span></span>    |
|<span data-ttu-id="3e1c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e1c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e1c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-113">Not supported.</span></span>    |
|<span data-ttu-id="3e1c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e1c3-114">Application</span></span> | <span data-ttu-id="3e1c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e1c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e1c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="3e1c3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e1c3-117">Request headers</span></span>
| <span data-ttu-id="3e1c3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3e1c3-118">Name</span></span>       | <span data-ttu-id="3e1c3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3e1c3-119">Type</span></span> | <span data-ttu-id="3e1c3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1c3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3e1c3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e1c3-121">Authorization</span></span>  | <span data-ttu-id="3e1c3-122">string</span><span class="sxs-lookup"><span data-stu-id="3e1c3-122">string</span></span>  | <span data-ttu-id="3e1c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e1c3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e1c3-125">Request body</span></span>
<span data-ttu-id="3e1c3-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e1c3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e1c3-129">Property</span></span>     | <span data-ttu-id="3e1c3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e1c3-130">Type</span></span>   |<span data-ttu-id="3e1c3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1c3-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="3e1c3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1c3-132">Response</span></span>

<span data-ttu-id="3e1c3-133">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e1c3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3e1c3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e1c3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e1c3-135">Request</span></span>
<span data-ttu-id="3e1c3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e1c3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e1c3-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e1c3-138">C#</span><span class="sxs-lookup"><span data-stu-id="3e1c3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e1c3-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e1c3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e1c3-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3e1c3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3e1c3-141">Java</span><span class="sxs-lookup"><span data-stu-id="3e1c3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3e1c3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1c3-142">Response</span></span>
<span data-ttu-id="3e1c3-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1c3-143">Here is an example of the response.</span></span>
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
