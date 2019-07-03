---
title: Создание раздела
description: Создание нового Оненотесектион в указанной записной книжке.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: a84ee9373b6137ee0bbafbe05c0c97c351b340b8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454715"
---
# <a name="create-section"></a><span data-ttu-id="317ff-103">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="317ff-103">Create section</span></span>

<span data-ttu-id="317ff-104">Создание нового [оненотесектион](../resources/section.md) в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="317ff-104">Create a new [onenoteSection](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="317ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="317ff-105">Permissions</span></span>
<span data-ttu-id="317ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="317ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="317ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="317ff-108">Permission type</span></span>      | <span data-ttu-id="317ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="317ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="317ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="317ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="317ff-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="317ff-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="317ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="317ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="317ff-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="317ff-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="317ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="317ff-114">Application</span></span> | <span data-ttu-id="317ff-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="317ff-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="317ff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="317ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="317ff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="317ff-117">Request headers</span></span>
| <span data-ttu-id="317ff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="317ff-118">Name</span></span>       | <span data-ttu-id="317ff-119">Тип</span><span class="sxs-lookup"><span data-stu-id="317ff-119">Type</span></span> | <span data-ttu-id="317ff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="317ff-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="317ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="317ff-121">Authorization</span></span>  | <span data-ttu-id="317ff-122">string</span><span class="sxs-lookup"><span data-stu-id="317ff-122">string</span></span>  | <span data-ttu-id="317ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="317ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="317ff-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="317ff-125">Content-Type</span></span> | <span data-ttu-id="317ff-126">string</span><span class="sxs-lookup"><span data-stu-id="317ff-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="317ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="317ff-127">Request body</span></span>
<span data-ttu-id="317ff-128">В тексте запроса укажите имя раздела.</span><span class="sxs-lookup"><span data-stu-id="317ff-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="317ff-p103">В рамках одного и того же уровня иерархии имена разделов должны быть уникальными. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="317ff-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="317ff-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="317ff-131">Response</span></span>

<span data-ttu-id="317ff-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [оненотесектион](../resources/section.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="317ff-132">If successful, this method returns a `201 Created` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="317ff-133">Пример</span><span class="sxs-lookup"><span data-stu-id="317ff-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="317ff-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="317ff-134">Request</span></span>
<span data-ttu-id="317ff-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="317ff-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="317ff-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="317ff-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="317ff-137">C#</span><span class="sxs-lookup"><span data-stu-id="317ff-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-section-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="317ff-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="317ff-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-section-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="317ff-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="317ff-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-section-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="317ff-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="317ff-140">Response</span></span>
<span data-ttu-id="317ff-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="317ff-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
