---
author: swapnil1993
ms.date: 08/30/2020
title: Создание columnDefinition в типе контента
description: Добавление столбца в тип контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 7071322064d55c21123fabd5ddc80d63fa5575ac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946966"
---
# <a name="create-columndefinition-for-a-content-type"></a><span data-ttu-id="9752f-103">Создание columnDefinition для типа контента</span><span class="sxs-lookup"><span data-stu-id="9752f-103">Create columnDefinition for a content type</span></span>
<span data-ttu-id="9752f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9752f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9752f-105">Добавление столбца в [тип контента.][contentType] in a site or list by specifying a [columnDefinition][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="9752f-105">Add a column to a [content type][contentType] in a site or list by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="9752f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9752f-106">Permissions</span></span>

<span data-ttu-id="9752f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9752f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="9752f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9752f-109">Permission type</span></span> | <span data-ttu-id="9752f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9752f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9752f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9752f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9752f-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9752f-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="9752f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9752f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9752f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9752f-114">Not supported.</span></span> |
|<span data-ttu-id="9752f-115">Application</span><span class="sxs-lookup"><span data-stu-id="9752f-115">Application</span></span> | <span data-ttu-id="9752f-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9752f-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="9752f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9752f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="9752f-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9752f-118">Request body</span></span>

<span data-ttu-id="9752f-119">В теле запроса добавьте представление JSON ресурса [columnDefinition.][]</span><span class="sxs-lookup"><span data-stu-id="9752f-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="9752f-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="9752f-120">Response</span></span>

<span data-ttu-id="9752f-121">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9752f-121">If successful, this method returns a `200 OK` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9752f-122">Пример</span><span class="sxs-lookup"><span data-stu-id="9752f-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="9752f-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="9752f-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a><span data-ttu-id="9752f-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="9752f-124">Response</span></span>

<span data-ttu-id="9752f-125">Ответ возвращает столбец, добавленный в тип контента.</span><span class="sxs-lookup"><span data-stu-id="9752f-125">The response returns the column added to a content type.</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
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
  

