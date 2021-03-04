---
author: swapnil1993
ms.date: 08/30/2020
title: Создание columnDefinition
description: Добавление столбца в тип контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 071a855c79c055179022157b991b4a9f2789cad1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447230"
---
# <a name="create-columndefinition"></a><span data-ttu-id="d690f-103">Создание columnDefinition</span><span class="sxs-lookup"><span data-stu-id="d690f-103">Create columnDefinition</span></span>
<span data-ttu-id="d690f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d690f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="d690f-105">Добавляет существующий столбец [столбец]сайта или[спискаDefinition] в [контент типа][контентаType.]</span><span class="sxs-lookup"><span data-stu-id="d690f-105">Adds existing site or list [column][columnDefinition] to a [content type][contentType].</span></span>

## <a name="permissions"></a><span data-ttu-id="d690f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d690f-106">Permissions</span></span>

<span data-ttu-id="d690f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d690f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="d690f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d690f-109">Permission type</span></span> | <span data-ttu-id="d690f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d690f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d690f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d690f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d690f-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d690f-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="d690f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d690f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d690f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d690f-114">Not supported.</span></span> |
|<span data-ttu-id="d690f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d690f-115">Application</span></span> | <span data-ttu-id="d690f-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d690f-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="d690f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d690f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="d690f-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d690f-118">Request body</span></span>

<span data-ttu-id="d690f-119">В теле запроса добавьте представление JSON ресурса [columnDefinition.][]</span><span class="sxs-lookup"><span data-stu-id="d690f-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="d690f-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="d690f-120">Response</span></span>

<span data-ttu-id="d690f-121">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект contentType][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d690f-121">If successful, this method returns a `200 OK` response code and [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d690f-122">Пример</span><span class="sxs-lookup"><span data-stu-id="d690f-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="d690f-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="d690f-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a><span data-ttu-id="d690f-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="d690f-124">Response</span></span>

<span data-ttu-id="d690f-125">Ответ возвращает список всех столбцов, добавленных в тип контента.</span><span class="sxs-lookup"><span data-stu-id="d690f-125">The response returns a list of all columns added to a content type.</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true, "scopes": "sites.readwrite.all" } -->

  

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
  

