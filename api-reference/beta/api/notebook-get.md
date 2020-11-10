---
title: Вывод записной книжки
description: Получение свойств и связей объекта записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 67d1fbae81bc678f79d8c9f10ab3fcb4719dc56f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978305"
---
# <a name="get-notebook"></a><span data-ttu-id="18630-103">Вывод записной книжки</span><span class="sxs-lookup"><span data-stu-id="18630-103">Get notebook</span></span>

<span data-ttu-id="18630-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18630-105">Получение свойств и связей объекта [записной книжки](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="18630-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="18630-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18630-106">Permissions</span></span>
<span data-ttu-id="18630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18630-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18630-109">Permission type</span></span>      | <span data-ttu-id="18630-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18630-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18630-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18630-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18630-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18630-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="18630-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18630-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18630-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18630-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="18630-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18630-115">Application</span></span> | <span data-ttu-id="18630-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18630-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18630-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18630-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18630-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18630-118">Optional query parameters</span></span>
<span data-ttu-id="18630-119">Этот метод поддерживает `select` `expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="18630-119">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="18630-120">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="18630-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18630-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18630-121">Request headers</span></span>
| <span data-ttu-id="18630-122">Имя</span><span class="sxs-lookup"><span data-stu-id="18630-122">Name</span></span>       | <span data-ttu-id="18630-123">Тип</span><span class="sxs-lookup"><span data-stu-id="18630-123">Type</span></span> | <span data-ttu-id="18630-124">Описание</span><span class="sxs-lookup"><span data-stu-id="18630-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18630-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18630-125">Authorization</span></span>  | <span data-ttu-id="18630-126">string</span><span class="sxs-lookup"><span data-stu-id="18630-126">string</span></span>  | <span data-ttu-id="18630-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18630-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18630-129">Accept</span><span class="sxs-lookup"><span data-stu-id="18630-129">Accept</span></span> | <span data-ttu-id="18630-130">строка</span><span class="sxs-lookup"><span data-stu-id="18630-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="18630-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18630-131">Request body</span></span>
<span data-ttu-id="18630-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18630-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18630-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="18630-133">Response</span></span>

<span data-ttu-id="18630-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18630-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18630-135">Пример</span><span class="sxs-lookup"><span data-stu-id="18630-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18630-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="18630-136">Request</span></span>
<span data-ttu-id="18630-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18630-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18630-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="18630-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
# <a name="c"></a>[<span data-ttu-id="18630-139">C#</span><span class="sxs-lookup"><span data-stu-id="18630-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18630-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18630-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18630-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18630-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18630-142">Java</span><span class="sxs-lookup"><span data-stu-id="18630-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18630-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="18630-143">Response</span></span>
<span data-ttu-id="18630-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18630-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
