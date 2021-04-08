---
author: swapnil1993
ms.date: 08/30/2020
title: Создание columnDefinition на сайте
description: Создание столбца сайта.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1404707dc2a98b4ac60e663fd25d595c977148f7
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638844"
---
# <a name="create-columndefinition-for-a-site"></a><span data-ttu-id="895bc-103">Создание columnDefinition для сайта</span><span class="sxs-lookup"><span data-stu-id="895bc-103">Create columnDefinition for a site</span></span>
<span data-ttu-id="895bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="895bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="895bc-105">Создание столбца для [сайта][site] by specifying a [columnDefinition][columnDefinition] .</span><span class="sxs-lookup"><span data-stu-id="895bc-105">Create a column for a [site][site] by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="895bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="895bc-106">Permissions</span></span>

<span data-ttu-id="895bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="895bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="895bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="895bc-109">Permission type</span></span> | <span data-ttu-id="895bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="895bc-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="895bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="895bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="895bc-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="895bc-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="895bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="895bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="895bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="895bc-114">Not supported.</span></span> |
|<span data-ttu-id="895bc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="895bc-115">Application</span></span> | <span data-ttu-id="895bc-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="895bc-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="895bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="895bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="895bc-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="895bc-118">Request body</span></span>

<span data-ttu-id="895bc-119">В теле запроса добавьте представление JSON ресурса [columnDefinition.][]</span><span class="sxs-lookup"><span data-stu-id="895bc-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="895bc-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="895bc-120">Response</span></span>

<span data-ttu-id="895bc-121">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект columnDefinition][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="895bc-121">If successful, this method returns a `201 Created` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="895bc-122">Пример</span><span class="sxs-lookup"><span data-stu-id="895bc-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="895bc-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="895bc-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/columns
Content-Type: application/json

{
   "description":"test",
   "enforceUniqueValues":false,
   "hidden":false,
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

### <a name="response"></a><span data-ttu-id="895bc-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="895bc-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "description":"test",
   "displayName":"Title",
   "enforceUniqueValues":false,
   "hidden":false,
   "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
  

