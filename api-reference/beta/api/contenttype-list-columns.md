---
author: swapnil1993
title: Список columnDefinitions в типе контента
description: Список столбцов в типе контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 49a47efbeb59869dfc4f1b83946f9b6a8f178924
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468910"
---
# <a name="list-columns-in-a-content-type"></a><span data-ttu-id="531cf-103">Список столбцов в типе контента</span><span class="sxs-lookup"><span data-stu-id="531cf-103">List columns in a content type</span></span>
<span data-ttu-id="531cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="531cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="531cf-105">Получите коллекцию столбцов, представленную в качестве [ресурсов columnDefinitionDefinition,][] в [типе контента.][contentType]</span><span class="sxs-lookup"><span data-stu-id="531cf-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [content type][contentType].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="531cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="531cf-106">Permissions</span></span>

  

<span data-ttu-id="531cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="531cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="531cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="531cf-109">Permission type</span></span> | <span data-ttu-id="531cf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="531cf-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="531cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="531cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="531cf-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="531cf-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="531cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="531cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="531cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531cf-114">Not supported.</span></span> |
|<span data-ttu-id="531cf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="531cf-115">Application</span></span> | <span data-ttu-id="531cf-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="531cf-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="531cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="531cf-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}/columns
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="531cf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="531cf-118">Optional query parameters</span></span>
<span data-ttu-id="531cf-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="531cf-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="531cf-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="531cf-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="531cf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="531cf-121">Request headers</span></span>
|<span data-ttu-id="531cf-122">Имя</span><span class="sxs-lookup"><span data-stu-id="531cf-122">Name</span></span>|<span data-ttu-id="531cf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="531cf-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="531cf-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="531cf-124">Authorization</span></span>|<span data-ttu-id="531cf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="531cf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="531cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="531cf-127">Request body</span></span>
<span data-ttu-id="531cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="531cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="531cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="531cf-129">Response</span></span>

<span data-ttu-id="531cf-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="531cf-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="531cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="531cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="531cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="531cf-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="531cf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="531cf-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_contenttype" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="531cf-134">C#</span><span class="sxs-lookup"><span data-stu-id="531cf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="531cf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="531cf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="531cf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="531cf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="531cf-137">Java</span><span class="sxs-lookup"><span data-stu-id="531cf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="531cf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="531cf-138">Response</span></span>
><span data-ttu-id="531cf-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="531cf-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "value":[
      {
         "description":"",
         "displayName":"Title",
         "hidden":false,
         "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Title",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      },
      {
         "description":"",
         "displayName":"Address",
         "id":"11dfef35-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Address",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      }
   ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
 
