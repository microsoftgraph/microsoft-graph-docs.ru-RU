---
title: Создание sectionGroup
description: Создание группы разделов в указанной группе разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: d8b5c01d03e88f24641c2e900351bd58d7bf6054
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320016"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="77b1a-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="77b1a-103">Create sectionGroup</span></span>

<span data-ttu-id="77b1a-104">Создание [группы разделов](../resources/sectiongroup.md) в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77b1a-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="77b1a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77b1a-105">Permissions</span></span>
<span data-ttu-id="77b1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77b1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77b1a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77b1a-108">Permission type</span></span>      | <span data-ttu-id="77b1a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77b1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77b1a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77b1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77b1a-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77b1a-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="77b1a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77b1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77b1a-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77b1a-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="77b1a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77b1a-114">Application</span></span> | <span data-ttu-id="77b1a-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77b1a-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77b1a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77b1a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="77b1a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77b1a-117">Request headers</span></span>
| <span data-ttu-id="77b1a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="77b1a-118">Name</span></span>       | <span data-ttu-id="77b1a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="77b1a-119">Type</span></span> | <span data-ttu-id="77b1a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="77b1a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77b1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="77b1a-121">Authorization</span></span>  | <span data-ttu-id="77b1a-122">string</span><span class="sxs-lookup"><span data-stu-id="77b1a-122">string</span></span>  | <span data-ttu-id="77b1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77b1a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77b1a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77b1a-125">Content-Type</span></span> | <span data-ttu-id="77b1a-126">string</span><span class="sxs-lookup"><span data-stu-id="77b1a-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="77b1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77b1a-127">Request body</span></span>
<span data-ttu-id="77b1a-128">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77b1a-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="77b1a-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="77b1a-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="77b1a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="77b1a-131">Response</span></span>

<span data-ttu-id="77b1a-132">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77b1a-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77b1a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="77b1a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77b1a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="77b1a-134">Request</span></span>
<span data-ttu-id="77b1a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77b1a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="77b1a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="77b1a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77b1a-137">C#</span><span class="sxs-lookup"><span data-stu-id="77b1a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77b1a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77b1a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77b1a-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77b1a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77b1a-140">Java</span><span class="sxs-lookup"><span data-stu-id="77b1a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77b1a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="77b1a-141">Response</span></span>
<span data-ttu-id="77b1a-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77b1a-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
