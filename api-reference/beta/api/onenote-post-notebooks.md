---
title: Создание записной книжки
description: Создание записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 8bed7897875adb722262441ef34618afb271ef7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456546"
---
# <a name="create-notebook"></a><span data-ttu-id="04472-103">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="04472-103">Create notebook</span></span>

<span data-ttu-id="04472-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04472-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04472-105">Создайте новую [записную книжку](../resources/notebook.md)OneNote.</span><span class="sxs-lookup"><span data-stu-id="04472-105">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="04472-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04472-106">Permissions</span></span>
<span data-ttu-id="04472-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04472-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04472-109">Permission type</span></span>      | <span data-ttu-id="04472-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04472-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04472-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04472-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04472-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04472-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="04472-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04472-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04472-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04472-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="04472-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04472-115">Application</span></span> | <span data-ttu-id="04472-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04472-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04472-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04472-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="04472-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04472-118">Request headers</span></span>
| <span data-ttu-id="04472-119">Имя</span><span class="sxs-lookup"><span data-stu-id="04472-119">Name</span></span>       | <span data-ttu-id="04472-120">Тип</span><span class="sxs-lookup"><span data-stu-id="04472-120">Type</span></span> | <span data-ttu-id="04472-121">Описание</span><span class="sxs-lookup"><span data-stu-id="04472-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04472-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04472-122">Authorization</span></span>  | <span data-ttu-id="04472-123">string</span><span class="sxs-lookup"><span data-stu-id="04472-123">string</span></span>  | <span data-ttu-id="04472-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04472-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04472-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04472-126">Content-Type</span></span> | <span data-ttu-id="04472-127">string</span><span class="sxs-lookup"><span data-stu-id="04472-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="04472-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04472-128">Request body</span></span>
<span data-ttu-id="04472-129">В тексте запроса укажите имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="04472-129">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="04472-130">Имена записных книжек должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="04472-130">Notebook names must be unique.</span></span> <span data-ttu-id="04472-131">Имя не может содержать более 128 символов или содержать следующие символы:? \*\/: <>| ' "</span><span class="sxs-lookup"><span data-stu-id="04472-131">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="04472-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="04472-132">Response</span></span>

<span data-ttu-id="04472-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [записной книжки](../resources/notebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04472-133">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04472-134">Пример</span><span class="sxs-lookup"><span data-stu-id="04472-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04472-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="04472-135">Request</span></span>
<span data-ttu-id="04472-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04472-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04472-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="04472-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```
# <a name="c"></a>[<span data-ttu-id="04472-138">C#</span><span class="sxs-lookup"><span data-stu-id="04472-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-notebook-from-onenote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04472-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04472-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notebook-from-onenote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04472-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04472-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-notebook-from-onenote-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04472-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="04472-141">Response</span></span>
<span data-ttu-id="04472-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04472-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
