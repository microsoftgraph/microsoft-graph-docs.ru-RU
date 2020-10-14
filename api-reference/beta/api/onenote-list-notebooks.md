---
title: Список записных книжек
description: Получение списка объектов записных книжек.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b8f4f243b6cc57f0db0c41244da897e3138f380a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460000"
---
# <a name="list-notebooks"></a><span data-ttu-id="4abbc-103">Список записных книжек</span><span class="sxs-lookup"><span data-stu-id="4abbc-103">List notebooks</span></span>

<span data-ttu-id="4abbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4abbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4abbc-105">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="4abbc-105">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4abbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4abbc-106">Permissions</span></span>
<span data-ttu-id="4abbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4abbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4abbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4abbc-109">Permission type</span></span>      | <span data-ttu-id="4abbc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4abbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4abbc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4abbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4abbc-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4abbc-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4abbc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4abbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4abbc-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4abbc-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4abbc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4abbc-115">Application</span></span> | <span data-ttu-id="4abbc-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4abbc-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4abbc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4abbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4abbc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4abbc-118">Optional query parameters</span></span>
<span data-ttu-id="4abbc-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4abbc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="4abbc-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="4abbc-120">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="4abbc-121">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="4abbc-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4abbc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4abbc-122">Request headers</span></span>
| <span data-ttu-id="4abbc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4abbc-123">Name</span></span>       | <span data-ttu-id="4abbc-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4abbc-124">Type</span></span> | <span data-ttu-id="4abbc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4abbc-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4abbc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4abbc-126">Authorization</span></span>  | <span data-ttu-id="4abbc-127">string</span><span class="sxs-lookup"><span data-stu-id="4abbc-127">string</span></span>  | <span data-ttu-id="4abbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4abbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4abbc-130">Accept</span><span class="sxs-lookup"><span data-stu-id="4abbc-130">Accept</span></span> | <span data-ttu-id="4abbc-131">строка</span><span class="sxs-lookup"><span data-stu-id="4abbc-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4abbc-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4abbc-132">Request body</span></span>
<span data-ttu-id="4abbc-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4abbc-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4abbc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4abbc-134">Response</span></span>

<span data-ttu-id="4abbc-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4abbc-135">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4abbc-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4abbc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4abbc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4abbc-137">Request</span></span>
<span data-ttu-id="4abbc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4abbc-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4abbc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4abbc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
# <a name="c"></a>[<span data-ttu-id="4abbc-140">C#</span><span class="sxs-lookup"><span data-stu-id="4abbc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4abbc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4abbc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4abbc-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4abbc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4abbc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4abbc-143">Response</span></span>
<span data-ttu-id="4abbc-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4abbc-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
