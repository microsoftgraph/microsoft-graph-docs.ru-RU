---
title: Обновление фотографии
description: Обновление свойств объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: 1f71679f09bc4b96b3640d0b37587e2675c93a57
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268392"
---
# <a name="update-photo"></a><span data-ttu-id="2342b-103">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="2342b-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2342b-104">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="2342b-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2342b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2342b-105">Permissions</span></span>
<span data-ttu-id="2342b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2342b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2342b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2342b-108">Permission type</span></span>      | <span data-ttu-id="2342b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2342b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2342b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2342b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2342b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2342b-111">Not supported.</span></span>    |
|<span data-ttu-id="2342b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2342b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2342b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2342b-113">Not supported.</span></span>    |
|<span data-ttu-id="2342b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2342b-114">Application</span></span> | <span data-ttu-id="2342b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2342b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2342b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2342b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="2342b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2342b-117">Request headers</span></span>
| <span data-ttu-id="2342b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2342b-118">Name</span></span>       | <span data-ttu-id="2342b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2342b-119">Type</span></span> | <span data-ttu-id="2342b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2342b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2342b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2342b-121">Authorization</span></span>  | <span data-ttu-id="2342b-122">string</span><span class="sxs-lookup"><span data-stu-id="2342b-122">string</span></span>  | <span data-ttu-id="2342b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2342b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2342b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2342b-125">Request body</span></span>
<span data-ttu-id="2342b-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2342b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2342b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2342b-129">Property</span></span>     | <span data-ttu-id="2342b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2342b-130">Type</span></span>   |<span data-ttu-id="2342b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2342b-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="2342b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2342b-132">Response</span></span>

<span data-ttu-id="2342b-133">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2342b-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2342b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2342b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2342b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2342b-135">Request</span></span>
<span data-ttu-id="2342b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2342b-136">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2342b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2342b-137">Response</span></span>
<span data-ttu-id="2342b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2342b-138">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2342b-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2342b-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2342b-140">C#</span><span class="sxs-lookup"><span data-stu-id="2342b-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2342b-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="2342b-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_photo-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2342b-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2342b-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_photo-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/photo-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/photo-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/photo-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
