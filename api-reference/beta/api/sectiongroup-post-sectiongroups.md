---
title: Создание sectionGroup
description: Создание группы разделов в указанной группе разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: cd8fa08f61c2dbe980741eaaf4f9cbcc5a2c3018
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976828"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="78f66-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="78f66-103">Create sectionGroup</span></span>

<span data-ttu-id="78f66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78f66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f66-105">Создание [группы разделов](../resources/sectiongroup.md) в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="78f66-105">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="78f66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78f66-106">Permissions</span></span>
<span data-ttu-id="78f66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78f66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78f66-109">Permission type</span></span>      | <span data-ttu-id="78f66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78f66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78f66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78f66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="78f66-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f66-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="78f66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78f66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f66-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78f66-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="78f66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78f66-115">Application</span></span> | <span data-ttu-id="78f66-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f66-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78f66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78f66-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="78f66-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78f66-118">Request headers</span></span>
| <span data-ttu-id="78f66-119">Имя</span><span class="sxs-lookup"><span data-stu-id="78f66-119">Name</span></span>       | <span data-ttu-id="78f66-120">Тип</span><span class="sxs-lookup"><span data-stu-id="78f66-120">Type</span></span> | <span data-ttu-id="78f66-121">Описание</span><span class="sxs-lookup"><span data-stu-id="78f66-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78f66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f66-122">Authorization</span></span>  | <span data-ttu-id="78f66-123">string</span><span class="sxs-lookup"><span data-stu-id="78f66-123">string</span></span>  | <span data-ttu-id="78f66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78f66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78f66-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78f66-126">Content-Type</span></span> | <span data-ttu-id="78f66-127">string</span><span class="sxs-lookup"><span data-stu-id="78f66-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="78f66-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78f66-128">Request body</span></span>
<span data-ttu-id="78f66-129">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="78f66-129">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="78f66-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="78f66-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="78f66-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="78f66-132">Response</span></span>

<span data-ttu-id="78f66-133">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="78f66-133">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f66-134">Пример</span><span class="sxs-lookup"><span data-stu-id="78f66-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78f66-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="78f66-135">Request</span></span>
<span data-ttu-id="78f66-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78f66-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78f66-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="78f66-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="78f66-138">C#</span><span class="sxs-lookup"><span data-stu-id="78f66-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78f66-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78f66-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78f66-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78f66-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78f66-141">Java</span><span class="sxs-lookup"><span data-stu-id="78f66-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sectiongroup-from-sectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="78f66-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="78f66-142">Response</span></span>
<span data-ttu-id="78f66-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78f66-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


