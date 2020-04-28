---
title: Создание sectionGroup
description: Создайте новую группу разделов в указанной записной книжке.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e9dc9992f05ae2fac9234b3431817ce655bbd06b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456700"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="d309d-103">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="d309d-103">Create sectionGroup</span></span>

<span data-ttu-id="d309d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d309d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d309d-105">Создайте новую [группу разделов](../resources/sectiongroup.md) в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="d309d-105">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="d309d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d309d-106">Permissions</span></span>
<span data-ttu-id="d309d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d309d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d309d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d309d-109">Permission type</span></span>      | <span data-ttu-id="d309d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d309d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d309d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d309d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d309d-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d309d-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d309d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d309d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d309d-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d309d-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d309d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d309d-115">Application</span></span> | <span data-ttu-id="d309d-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d309d-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d309d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d309d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="d309d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d309d-118">Request headers</span></span>
| <span data-ttu-id="d309d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d309d-119">Name</span></span>       | <span data-ttu-id="d309d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d309d-120">Type</span></span> | <span data-ttu-id="d309d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d309d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d309d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d309d-122">Authorization</span></span>  | <span data-ttu-id="d309d-123">string</span><span class="sxs-lookup"><span data-stu-id="d309d-123">string</span></span>  | <span data-ttu-id="d309d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d309d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d309d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d309d-126">Content-Type</span></span> | <span data-ttu-id="d309d-127">string</span><span class="sxs-lookup"><span data-stu-id="d309d-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d309d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d309d-128">Request body</span></span>
<span data-ttu-id="d309d-129">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="d309d-129">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="d309d-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="d309d-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="d309d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d309d-132">Response</span></span>

<span data-ttu-id="d309d-133">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d309d-133">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d309d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d309d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d309d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d309d-135">Request</span></span>
<span data-ttu-id="d309d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d309d-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d309d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d309d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
# <a name="c"></a>[<span data-ttu-id="d309d-138">C#</span><span class="sxs-lookup"><span data-stu-id="d309d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sectiongroup-from-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d309d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d309d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sectiongroup-from-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d309d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d309d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sectiongroup-from-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d309d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d309d-141">Response</span></span>
<span data-ttu-id="d309d-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d309d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
