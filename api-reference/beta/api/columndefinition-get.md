---
author: swapnil1993
title: Получить columnDefinition
description: " Получите столбец типа сайта, списка или контента."
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f2e9bbca28dd0096401a2c59b92d5a26e35ee75e
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401402"
---
# <a name="get-columndefinition"></a><span data-ttu-id="edf75-103">Получить columnDefinition</span><span class="sxs-lookup"><span data-stu-id="edf75-103">Get columnDefinition</span></span>
<span data-ttu-id="edf75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edf75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="edf75-105">Извлечение метаданных для [столбца сайта,][] [списка][] [или contentType.][] [][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="edf75-105">Retrieve the metadata for a [site][], [list][] or [contentType][] [column][columnDefinition].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="edf75-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edf75-106">Permissions</span></span>

  

<span data-ttu-id="edf75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="edf75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="edf75-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edf75-109">Permission type</span></span> | <span data-ttu-id="edf75-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edf75-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edf75-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edf75-111">Delegated (work or school account)</span></span> | <span data-ttu-id="edf75-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="edf75-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="edf75-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edf75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edf75-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edf75-114">Not supported.</span></span> |
|<span data-ttu-id="edf75-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="edf75-115">Application</span></span> | <span data-ttu-id="edf75-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="edf75-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="edf75-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edf75-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /sites/{site-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/columns/{column-id}
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a><span data-ttu-id="edf75-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edf75-118">Request headers</span></span>
|<span data-ttu-id="edf75-119">Имя</span><span class="sxs-lookup"><span data-stu-id="edf75-119">Name</span></span>|<span data-ttu-id="edf75-120">Описание</span><span class="sxs-lookup"><span data-stu-id="edf75-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="edf75-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edf75-121">Authorization</span></span>|<span data-ttu-id="edf75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edf75-p102">Bearer {token}. Required.</span></span>|  

## <a name="request-body"></a><span data-ttu-id="edf75-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="edf75-124">Request body</span></span>

  

<span data-ttu-id="edf75-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edf75-125">Do not supply a request body with this method.</span></span>

  

## <a name="example"></a><span data-ttu-id="edf75-126">Пример</span><span class="sxs-lookup"><span data-stu-id="edf75-126">Example</span></span>

  

### <a name="request"></a><span data-ttu-id="edf75-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="edf75-127">Request</span></span>

  


# <a name="http"></a>[<span data-ttu-id="edf75-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="edf75-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```msgraph-interactive
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[<span data-ttu-id="edf75-129">C#</span><span class="sxs-lookup"><span data-stu-id="edf75-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-column-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edf75-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edf75-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-column-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edf75-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edf75-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-column-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edf75-132">Java</span><span class="sxs-lookup"><span data-stu-id="edf75-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-column-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


  

### <a name="response"></a><span data-ttu-id="edf75-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="edf75-133">Response</span></span>

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
