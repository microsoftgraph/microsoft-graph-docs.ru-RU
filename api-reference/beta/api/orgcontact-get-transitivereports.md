---
title: Get transitiveReports for orgContact
description: Получите количество транзитных отчетов для организационного контакта.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43a3d7736d33a1ca21ccf881dba92275dde553a8
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151781"
---
# <a name="get-transitivereports-for-orgcontact"></a><span data-ttu-id="40813-103">Get transitiveReports for orgContact</span><span class="sxs-lookup"><span data-stu-id="40813-103">Get transitiveReports for orgContact</span></span>

<span data-ttu-id="40813-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40813-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40813-105">Извлечение графа транзитных отчетов для организационного контакта.</span><span class="sxs-lookup"><span data-stu-id="40813-105">Retrieve a count of transitive reports for an organizational contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="40813-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40813-106">Permissions</span></span>

<span data-ttu-id="40813-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="40813-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40813-109">Permission type</span></span> | <span data-ttu-id="40813-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40813-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="40813-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40813-111">Delegated (work or school account)</span></span> | <span data-ttu-id="40813-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="40813-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="40813-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40813-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40813-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40813-114">Not supported.</span></span> |
| <span data-ttu-id="40813-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40813-115">Application</span></span> | <span data-ttu-id="40813-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="40813-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40813-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40813-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/transitiveReports/$count
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40813-118">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="40813-118">Optional query parameters</span></span>

<span data-ttu-id="40813-119">Этот метод не поддерживает использование параметров запроса, но требует `$count` сегмента запросов.</span><span class="sxs-lookup"><span data-stu-id="40813-119">This method does not support the use of query parameters, but does require the `$count` query segment.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40813-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40813-120">Request headers</span></span>

| <span data-ttu-id="40813-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40813-121">Header</span></span>       | <span data-ttu-id="40813-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40813-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40813-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40813-123">Authorization</span></span>  | <span data-ttu-id="40813-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40813-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40813-126">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="40813-126">ConsistencyLevel</span></span> | <span data-ttu-id="40813-127">необязательный.</span><span class="sxs-lookup"><span data-stu-id="40813-127">eventual.</span></span> <span data-ttu-id="40813-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="40813-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40813-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40813-129">Request body</span></span>

<span data-ttu-id="40813-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40813-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40813-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="40813-131">Response</span></span>

<span data-ttu-id="40813-132">В случае успешной работы этот метод возвращает код ответа и количество транзитных отчетов для организационного контакта `200 OK` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="40813-132">If successful, this method returns a `200 OK` response code and a count of transitive reports for an organizational contact in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40813-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="40813-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40813-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="40813-134">Request</span></span>

<span data-ttu-id="40813-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40813-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivereports"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```

### <a name="response"></a><span data-ttu-id="40813-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="40813-136">Response</span></span>

<span data-ttu-id="40813-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40813-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="40813-138">5 </span><span class="sxs-lookup"><span data-stu-id="40813-138">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
