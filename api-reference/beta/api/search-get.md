---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d7b84fdad96530f88f09c7da7b00a6013b19017e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938388"
---
# <a name="search"></a><span data-ttu-id="ba7a6-103">Поиск</span><span class="sxs-lookup"><span data-stu-id="ba7a6-103">Search</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba7a6-104">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="ba7a6-105">Он не работает как другой ресурс в Graph, но служит в качестве привязки к действиям поиска (запрос).</span><span class="sxs-lookup"><span data-stu-id="ba7a6-105">It does not behave as any other resource in Graph, but serves as an anchor to Search actions (Query).</span></span> <span data-ttu-id="ba7a6-106">В графике нет представления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-106">It has no resource representation in graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba7a6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba7a6-107">Permissions</span></span>

<span data-ttu-id="ba7a6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba7a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba7a6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba7a6-110">Permission type</span></span>                        | <span data-ttu-id="ba7a6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba7a6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba7a6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba7a6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba7a6-113">Mail. Read, Files. Read. ALL, Calendars. Read, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ba7a6-113">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="ba7a6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba7a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba7a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-115">Not supported.</span></span> |
| <span data-ttu-id="ba7a6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba7a6-116">Application</span></span>                            | <span data-ttu-id="ba7a6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba7a6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba7a6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a><span data-ttu-id="ba7a6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba7a6-119">Request headers</span></span>

| <span data-ttu-id="ba7a6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ba7a6-120">Name</span></span>      |<span data-ttu-id="ba7a6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ba7a6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba7a6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba7a6-122">Authorization</span></span> | <span data-ttu-id="ba7a6-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ba7a6-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba7a6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba7a6-124">Request body</span></span>

<span data-ttu-id="ba7a6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba7a6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba7a6-126">Response</span></span>

<span data-ttu-id="ba7a6-127">Этот ресурс не должен вызываться таким образом.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-127">This resource is not expected to be called as such.</span></span> <span data-ttu-id="ba7a6-128">Любой запрос к ресурсу повлечет некорректный запрос.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-128">Any request on the resource will incur a Bad Request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba7a6-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ba7a6-129">Next steps</span></span>

- <span data-ttu-id="ba7a6-130">Изучите действие [/Query](search-query.md) для поиска.</span><span class="sxs-lookup"><span data-stu-id="ba7a6-130">Explore the [/query](search-query.md) action on Search.</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
