---
author: swapnil1993
ms.date: 08/30/2020
title: Создание columnDefinition в списке
description: Создание столбца списка.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: c2f49b6b5ec25e6c2941e94d06c8b0b242a98447
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965165"
---
# <a name="create-columndefinition-for-a-list"></a><span data-ttu-id="cec79-103">Создание columnDefinition для списка</span><span class="sxs-lookup"><span data-stu-id="cec79-103">Create columnDefinition for a list</span></span>
<span data-ttu-id="cec79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cec79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="cec79-105">Создание столбца для [списка][list] by specifying a [columnDefinition][columnDefinition] .</span><span class="sxs-lookup"><span data-stu-id="cec79-105">Create a column for a [list][list] by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="cec79-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cec79-106">Permissions</span></span>

<span data-ttu-id="cec79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cec79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="cec79-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cec79-109">Permission type</span></span> | <span data-ttu-id="cec79-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cec79-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cec79-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cec79-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cec79-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="cec79-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="cec79-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cec79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cec79-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec79-114">Not supported.</span></span> |
|<span data-ttu-id="cec79-115">Application</span><span class="sxs-lookup"><span data-stu-id="cec79-115">Application</span></span> | <span data-ttu-id="cec79-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="cec79-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="cec79-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cec79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/lists/{list-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="cec79-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cec79-118">Request body</span></span>

<span data-ttu-id="cec79-119">В теле запроса добавьте представление JSON ресурса [columnDefinition.][]</span><span class="sxs-lookup"><span data-stu-id="cec79-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="cec79-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="cec79-120">Response</span></span>

<span data-ttu-id="cec79-121">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cec79-121">If successful, this method returns a `201 Created` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec79-122">Пример</span><span class="sxs-lookup"><span data-stu-id="cec79-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="cec79-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="cec79-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/columns
Content-Type: application/json

{
  "description": "test",
  "enforceUniqueValues": false,
  "hidden": false,
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

### <a name="response"></a><span data-ttu-id="cec79-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="cec79-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "test",
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
[list]: ../resources/list.md
  

