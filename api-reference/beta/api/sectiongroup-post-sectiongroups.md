---
title: Создание sectionGroup
description: Создание группы разделов в указанной группе разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ff8f0a16fa5fdd3299feb8fe509d78023558408e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067624"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="d1e3f-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="d1e3f-103">Create sectionGroup</span></span>

<span data-ttu-id="d1e3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1e3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1e3f-105">Создание [группы разделов](../resources/sectiongroup.md) в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="d1e3f-105">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1e3f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e3f-106">Permissions</span></span>
<span data-ttu-id="d1e3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e3f-109">Permission type</span></span>      | <span data-ttu-id="d1e3f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1e3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1e3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1e3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1e3f-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e3f-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1e3f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1e3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1e3f-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1e3f-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d1e3f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1e3f-115">Application</span></span> | <span data-ttu-id="d1e3f-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e3f-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1e3f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1e3f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="d1e3f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1e3f-118">Request headers</span></span>
| <span data-ttu-id="d1e3f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d1e3f-119">Name</span></span>       | <span data-ttu-id="d1e3f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d1e3f-120">Type</span></span> | <span data-ttu-id="d1e3f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d1e3f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1e3f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1e3f-122">Authorization</span></span>  | <span data-ttu-id="d1e3f-123">string</span><span class="sxs-lookup"><span data-stu-id="d1e3f-123">string</span></span>  | <span data-ttu-id="d1e3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1e3f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1e3f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1e3f-126">Content-Type</span></span> | <span data-ttu-id="d1e3f-127">string</span><span class="sxs-lookup"><span data-stu-id="d1e3f-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d1e3f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1e3f-128">Request body</span></span>
<span data-ttu-id="d1e3f-129">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="d1e3f-129">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="d1e3f-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="d1e3f-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="d1e3f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e3f-132">Response</span></span>

<span data-ttu-id="d1e3f-133">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1e3f-133">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1e3f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d1e3f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1e3f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1e3f-135">Request</span></span>
<span data-ttu-id="d1e3f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1e3f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1e3f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e3f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="c"></a>[<span data-ttu-id="d1e3f-138">C#</span><span class="sxs-lookup"><span data-stu-id="d1e3f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1e3f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1e3f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1e3f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1e3f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d1e3f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e3f-141">Response</span></span>
<span data-ttu-id="d1e3f-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1e3f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


