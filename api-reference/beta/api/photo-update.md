---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 30f112599f7b95dc91454980946f5d10e10ae29f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455832"
---
# <a name="update-photo"></a><span data-ttu-id="1ca05-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="1ca05-103">Update photo</span></span>

<span data-ttu-id="1ca05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ca05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca05-105">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="1ca05-105">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ca05-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca05-106">Permissions</span></span>
<span data-ttu-id="1ca05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca05-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca05-109">Permission type</span></span>      | <span data-ttu-id="1ca05-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ca05-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ca05-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ca05-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ca05-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca05-112">Not supported.</span></span>    |
|<span data-ttu-id="1ca05-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ca05-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ca05-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca05-114">Not supported.</span></span>    |
|<span data-ttu-id="1ca05-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ca05-115">Application</span></span> | <span data-ttu-id="1ca05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca05-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ca05-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ca05-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="1ca05-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ca05-118">Request headers</span></span>
| <span data-ttu-id="1ca05-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1ca05-119">Name</span></span>       | <span data-ttu-id="1ca05-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1ca05-120">Type</span></span> | <span data-ttu-id="1ca05-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca05-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ca05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ca05-122">Authorization</span></span>  | <span data-ttu-id="1ca05-123">string</span><span class="sxs-lookup"><span data-stu-id="1ca05-123">string</span></span>  | <span data-ttu-id="1ca05-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca05-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ca05-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ca05-126">Request body</span></span>
<span data-ttu-id="1ca05-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1ca05-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1ca05-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ca05-130">Property</span></span>     | <span data-ttu-id="1ca05-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ca05-131">Type</span></span>   |<span data-ttu-id="1ca05-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca05-132">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="1ca05-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ca05-133">Response</span></span>

<span data-ttu-id="1ca05-134">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca05-134">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ca05-135">Пример</span><span class="sxs-lookup"><span data-stu-id="1ca05-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ca05-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ca05-136">Request</span></span>
<span data-ttu-id="1ca05-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ca05-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ca05-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ca05-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1ca05-139">C#</span><span class="sxs-lookup"><span data-stu-id="1ca05-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ca05-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ca05-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ca05-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ca05-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1ca05-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca05-142">Response</span></span>
<span data-ttu-id="1ca05-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca05-143">Here is an example of the response.</span></span>
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
