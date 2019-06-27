---
title: Создание sectionGroup
description: Создайте новую группу разделов в указанной записной книжке.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8d331040e4ee8d29b30402591408c15cf8e924e9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274517"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="a3151-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="a3151-103">Create sectionGroup</span></span>

<span data-ttu-id="a3151-104">Создайте новую [группу разделов](../resources/sectiongroup.md) в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="a3151-104">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3151-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3151-105">Permissions</span></span>
<span data-ttu-id="a3151-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3151-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3151-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3151-108">Permission type</span></span>      | <span data-ttu-id="a3151-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3151-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3151-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3151-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3151-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3151-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3151-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3151-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3151-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3151-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a3151-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3151-114">Application</span></span> | <span data-ttu-id="a3151-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3151-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3151-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3151-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="a3151-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3151-117">Request headers</span></span>
| <span data-ttu-id="a3151-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a3151-118">Name</span></span>       | <span data-ttu-id="a3151-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a3151-119">Type</span></span> | <span data-ttu-id="a3151-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3151-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3151-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3151-121">Authorization</span></span>  | <span data-ttu-id="a3151-122">string</span><span class="sxs-lookup"><span data-stu-id="a3151-122">string</span></span>  | <span data-ttu-id="a3151-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3151-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3151-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3151-125">Content-Type</span></span> | <span data-ttu-id="a3151-126">string</span><span class="sxs-lookup"><span data-stu-id="a3151-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a3151-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3151-127">Request body</span></span>
<span data-ttu-id="a3151-128">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="a3151-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="a3151-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="a3151-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="a3151-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3151-131">Response</span></span>

<span data-ttu-id="a3151-132">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3151-132">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3151-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a3151-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3151-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3151-134">Request</span></span>
<span data-ttu-id="a3151-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3151-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```

##### <a name="response"></a><span data-ttu-id="a3151-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3151-136">Response</span></span>
<span data-ttu-id="a3151-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3151-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a3151-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a3151-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a3151-141">C#</span><span class="sxs-lookup"><span data-stu-id="a3151-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_notebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3151-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3151-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_notebook-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a3151-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a3151-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_sectiongroup_from_notebook-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-post-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
