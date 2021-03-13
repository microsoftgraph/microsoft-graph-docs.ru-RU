---
author: swapnil1993
title: Обновление столбцаDefinition
description: Обновление столбца типа контента
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 89c26b5fcbe3f6509d2d763ed6e8e4d06a8530d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773349"
---
# <a name="update-columndefinition"></a><span data-ttu-id="1d6de-103">Обновление столбцаDefinition</span><span class="sxs-lookup"><span data-stu-id="1d6de-103">Update columnDefinition</span></span>
<span data-ttu-id="1d6de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d6de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="1d6de-105">Обновление [типа контента.][contentType] [column][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="1d6de-105">Update a [content type][contentType] [column][columnDefinition].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="1d6de-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d6de-106">Permissions</span></span>  

<span data-ttu-id="1d6de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d6de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="1d6de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d6de-109">Permission type</span></span> | <span data-ttu-id="1d6de-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d6de-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d6de-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d6de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d6de-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1d6de-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="1d6de-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d6de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d6de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d6de-114">Not supported.</span></span> |
|<span data-ttu-id="1d6de-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1d6de-115">Application</span></span> | <span data-ttu-id="1d6de-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1d6de-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="1d6de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d6de-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a><span data-ttu-id="1d6de-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d6de-118">Request headers</span></span>
|<span data-ttu-id="1d6de-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1d6de-119">Name</span></span>|<span data-ttu-id="1d6de-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1d6de-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d6de-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d6de-121">Authorization</span></span>|<span data-ttu-id="1d6de-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d6de-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d6de-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d6de-124">Content-Type</span></span>|<span data-ttu-id="1d6de-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d6de-p103">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="1d6de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d6de-127">Request body</span></span>

<span data-ttu-id="1d6de-128">В теле запроса предопределять представление JSON ресурса [columnDefinition][] для обновления.</span><span class="sxs-lookup"><span data-stu-id="1d6de-128">In the request body, supply a JSON representation of the [columnDefinition][] resource to update.</span></span>  

><span data-ttu-id="1d6de-129">**Примечание:** Обновить можно только необходимые и скрытые свойства.</span><span class="sxs-lookup"><span data-stu-id="1d6de-129">**Note:** Only required and hidden properties can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="1d6de-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d6de-130">Response</span></span>

<span data-ttu-id="1d6de-131">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1d6de-131">If successful, this method returns a `200 OK` response code and an updated [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d6de-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1d6de-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d6de-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d6de-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1d6de-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d6de-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype_column"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```
# <a name="c"></a>[<span data-ttu-id="1d6de-135">C#</span><span class="sxs-lookup"><span data-stu-id="1d6de-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contenttype-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d6de-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d6de-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d6de-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d6de-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d6de-138">Java</span><span class="sxs-lookup"><span data-stu-id="1d6de-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contenttype-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d6de-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d6de-139">Response</span></span>
><span data-ttu-id="1d6de-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d6de-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}

```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
