---
author: swapnil1993
title: Обновление столбцаDefinition
description: Обновление столбца типа сайта, списка или контента
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 90f9330fd5cb934ec5cead04cfcc245d46b172df
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952329"
---
# <a name="update-columndefinition"></a><span data-ttu-id="8a905-103">Обновление столбцаDefinition</span><span class="sxs-lookup"><span data-stu-id="8a905-103">Update columnDefinition</span></span>
<span data-ttu-id="8a905-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="8a905-105">Обновление [типа сайта,][] [списка][] [или контента.][contentType] [column][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="8a905-105">Update a [site][], [list][] or [content type][contentType] [column][columnDefinition].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="8a905-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a905-106">Permissions</span></span>  

<span data-ttu-id="8a905-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="8a905-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a905-109">Permission type</span></span> | <span data-ttu-id="8a905-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a905-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a905-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a905-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a905-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8a905-112">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="8a905-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a905-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a905-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a905-114">Not supported.</span></span> |
|<span data-ttu-id="8a905-115">Application</span><span class="sxs-lookup"><span data-stu-id="8a905-115">Application</span></span> | <span data-ttu-id="8a905-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8a905-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="8a905-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a905-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/columns/{column-id}
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a><span data-ttu-id="8a905-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a905-118">Request headers</span></span>
|<span data-ttu-id="8a905-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8a905-119">Name</span></span>|<span data-ttu-id="8a905-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8a905-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a905-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a905-121">Authorization</span></span>|<span data-ttu-id="8a905-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a905-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a905-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a905-124">Content-Type</span></span>|<span data-ttu-id="8a905-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a905-p103">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="8a905-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a905-127">Request body</span></span>

<span data-ttu-id="8a905-128">В теле запроса поставляем представление JSON этих свойств ресурса [columnDefinition][] для обновления.</span><span class="sxs-lookup"><span data-stu-id="8a905-128">In the request body, supply a JSON representation of those properties of a [columnDefinition][] resource to update.</span></span> <span data-ttu-id="8a905-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8a905-129">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="8a905-130">Для столбцов **в сайте** или списке **можно** обновить любое свойство **columnDefinition,** кроме **свойства id.**</span><span class="sxs-lookup"><span data-stu-id="8a905-130">For columns in **site** or **list**, you can update any property of **columnDefinition** other than the **id** property.</span></span>

<span data-ttu-id="8a905-131">Для столбцов **в contentType** можно обновить только **необходимое или** **скрытое** свойство.</span><span class="sxs-lookup"><span data-stu-id="8a905-131">For columns in **contentType**, you can update only the **required** or **hidden** property.</span></span>

## <a name="response"></a><span data-ttu-id="8a905-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a905-132">Response</span></span>

<span data-ttu-id="8a905-133">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8a905-133">If successful, this method returns a `200 OK` response code and an updated [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a905-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8a905-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a905-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a905-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8a905-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a905-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8a905-137">C#</span><span class="sxs-lookup"><span data-stu-id="8a905-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contenttype-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a905-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a905-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a905-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a905-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a905-140">Java</span><span class="sxs-lookup"><span data-stu-id="8a905-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contenttype-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a905-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a905-141">Response</span></span>
><span data-ttu-id="8a905-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a905-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
[list]: ../resources/list.md
[site]: ../resources/site.md

