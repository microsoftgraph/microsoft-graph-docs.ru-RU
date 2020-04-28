---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 64e9c65d0de415e62d0238c58dc460dd1a82fcd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453711"
---
# <a name="search"></a><span data-ttu-id="cb0b7-103">Поиск</span><span class="sxs-lookup"><span data-stu-id="cb0b7-103">Search</span></span>

<span data-ttu-id="cb0b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb0b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb0b7-105">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="cb0b7-106">Он не работает как другой ресурс в Graph, но служит в качестве привязки к действиям поиска (запрос).</span><span class="sxs-lookup"><span data-stu-id="cb0b7-106">It does not behave as any other resource in Graph, but serves as an anchor to Search actions (Query).</span></span> <span data-ttu-id="cb0b7-107">В графике нет представления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-107">It has no resource representation in graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="cb0b7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb0b7-108">Permissions</span></span>

<span data-ttu-id="cb0b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb0b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb0b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb0b7-111">Permission type</span></span>                        | <span data-ttu-id="cb0b7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb0b7-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb0b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb0b7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb0b7-114">Mail. Read, Files. Read. ALL, Calendars. Read, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="cb0b7-114">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="cb0b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb0b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb0b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-116">Not supported.</span></span> |
| <span data-ttu-id="cb0b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb0b7-117">Application</span></span>                            | <span data-ttu-id="cb0b7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb0b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb0b7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a><span data-ttu-id="cb0b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb0b7-120">Request headers</span></span>

| <span data-ttu-id="cb0b7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cb0b7-121">Name</span></span>      |<span data-ttu-id="cb0b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cb0b7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb0b7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb0b7-123">Authorization</span></span> | <span data-ttu-id="cb0b7-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="cb0b7-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb0b7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb0b7-125">Request body</span></span>

<span data-ttu-id="cb0b7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb0b7-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb0b7-127">Response</span></span>

<span data-ttu-id="cb0b7-128">Этот ресурс не должен вызываться таким образом.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-128">This resource is not expected to be called as such.</span></span> <span data-ttu-id="cb0b7-129">Любой запрос к ресурсу повлечет некорректный запрос.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-129">Any request on the resource will incur a Bad Request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cb0b7-130">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="cb0b7-130">Next steps</span></span>

- <span data-ttu-id="cb0b7-131">Изучите действие [/Query](search-query.md) для поиска.</span><span class="sxs-lookup"><span data-stu-id="cb0b7-131">Explore the [/query](search-query.md) action on Search.</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
