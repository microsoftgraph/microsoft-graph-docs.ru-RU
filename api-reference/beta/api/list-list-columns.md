---
author: swapnil1993
title: Столбцы спискаDefinitions в списке
description: Список столбцов в списке.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 7dd2b59086b930b0e7536033b662e61088b15372
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201075"
---
# <a name="list-columns-in-a-list"></a><span data-ttu-id="34848-103">Список столбцов в списке</span><span class="sxs-lookup"><span data-stu-id="34848-103">List columns in a list</span></span>
<span data-ttu-id="34848-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34848-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="34848-105">Получите коллекцию столбцов, представленных в качестве [столбцов ColumnDefinition][columnDefinition,] в [списке][list].</span><span class="sxs-lookup"><span data-stu-id="34848-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [list][list].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="34848-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34848-106">Permissions</span></span>

  

<span data-ttu-id="34848-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="34848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="34848-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34848-109">Permission type</span></span> | <span data-ttu-id="34848-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34848-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34848-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34848-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34848-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="34848-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="34848-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34848-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34848-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34848-114">Not supported.</span></span> |
|<span data-ttu-id="34848-115">Application</span><span class="sxs-lookup"><span data-stu-id="34848-115">Application</span></span> | <span data-ttu-id="34848-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="34848-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="34848-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34848-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http

GET /sites/{site-id}/lists/{list-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="34848-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34848-118">Optional query parameters</span></span>
<span data-ttu-id="34848-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="34848-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="34848-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="34848-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34848-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34848-121">Request headers</span></span>
|<span data-ttu-id="34848-122">Имя</span><span class="sxs-lookup"><span data-stu-id="34848-122">Name</span></span>|<span data-ttu-id="34848-123">Описание</span><span class="sxs-lookup"><span data-stu-id="34848-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="34848-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34848-124">Authorization</span></span>|<span data-ttu-id="34848-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34848-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34848-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34848-127">Request body</span></span>
<span data-ttu-id="34848-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34848-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34848-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="34848-129">Response</span></span>

<span data-ttu-id="34848-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="34848-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="34848-131">Пример</span><span class="sxs-lookup"><span data-stu-id="34848-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="34848-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34848-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="34848-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="34848-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_list" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="34848-134">C#</span><span class="sxs-lookup"><span data-stu-id="34848-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34848-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34848-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34848-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34848-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34848-137">Java</span><span class="sxs-lookup"><span data-stu-id="34848-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34848-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="34848-138">Response</span></span>
><span data-ttu-id="34848-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="34848-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.columnDefinition)"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "",
      "displayName": "Title",
      "hidden": false,
      "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
      "indexed": false,
      "name": "Title",
      "readOnly": false,
      "required": false,
      "text": {
        "allowMultipleLines": false,
        "appendChangesToExistingText": false,
        "linesForEditing": 0,
        "maxLength": 255
      }
    },
    {
      "description": "",
      "displayName": "Address",
      "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
      "indexed": false,
      "name": "Address",
      "readOnly": false,
      "required": false,
      "text": {
        "allowMultipleLines": false,
        "appendChangesToExistingText": false,
        "linesForEditing": 0,
        "maxLength": 255
      }
    }
  ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[list]: ../resources/list.md
 
