---
title: Вывод записной книжки
description: Получение свойств и связей объекта записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 8d2d716d99731cb6a3113fbc69a10efd907c3e74
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460791"
---
# <a name="get-notebook"></a><span data-ttu-id="6c03e-103">Вывод записной книжки</span><span class="sxs-lookup"><span data-stu-id="6c03e-103">Get notebook</span></span>

<span data-ttu-id="6c03e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c03e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c03e-105">Получение свойств и связей объекта [записной книжки](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="6c03e-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c03e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c03e-106">Permissions</span></span>
<span data-ttu-id="6c03e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c03e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c03e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c03e-109">Permission type</span></span>      | <span data-ttu-id="6c03e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c03e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c03e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c03e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6c03e-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c03e-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c03e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c03e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c03e-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c03e-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6c03e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c03e-115">Application</span></span> | <span data-ttu-id="6c03e-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c03e-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c03e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c03e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c03e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c03e-118">Optional query parameters</span></span>
<span data-ttu-id="6c03e-119">Этот метод поддерживает `select` `expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6c03e-119">This method supports the `select` and `expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="6c03e-120">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="6c03e-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c03e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c03e-121">Request headers</span></span>
| <span data-ttu-id="6c03e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6c03e-122">Name</span></span>       | <span data-ttu-id="6c03e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6c03e-123">Type</span></span> | <span data-ttu-id="6c03e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6c03e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c03e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c03e-125">Authorization</span></span>  | <span data-ttu-id="6c03e-126">string</span><span class="sxs-lookup"><span data-stu-id="6c03e-126">string</span></span>  | <span data-ttu-id="6c03e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c03e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c03e-129">Accept</span><span class="sxs-lookup"><span data-stu-id="6c03e-129">Accept</span></span> | <span data-ttu-id="6c03e-130">строка</span><span class="sxs-lookup"><span data-stu-id="6c03e-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6c03e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c03e-131">Request body</span></span>
<span data-ttu-id="6c03e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c03e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c03e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c03e-133">Response</span></span>

<span data-ttu-id="6c03e-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c03e-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c03e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="6c03e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c03e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c03e-136">Request</span></span>
<span data-ttu-id="6c03e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c03e-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c03e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c03e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
# <a name="c"></a>[<span data-ttu-id="6c03e-139">C#</span><span class="sxs-lookup"><span data-stu-id="6c03e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c03e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c03e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c03e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c03e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6c03e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c03e-142">Response</span></span>
<span data-ttu-id="6c03e-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c03e-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
