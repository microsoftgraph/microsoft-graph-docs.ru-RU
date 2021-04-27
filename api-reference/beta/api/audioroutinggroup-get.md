---
title: Получение группы маршрутизации звука
description: Извлечение свойств и связей объекта audioRoutingGroup.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cdb32816f05e9edd92850830627863fa72759229
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048017"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="731e8-103">Получение группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="731e8-103">Get audio routing group</span></span>

<span data-ttu-id="731e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="731e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="731e8-105">Извлечение свойств и связей [объекта audioRoutingGroup.](../resources/audioroutinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="731e8-105">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="731e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="731e8-106">Permissions</span></span>
<span data-ttu-id="731e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="731e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="731e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="731e8-109">Permission type</span></span>                        | <span data-ttu-id="731e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="731e8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="731e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="731e8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="731e8-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="731e8-112">Not Supported</span></span>                               |
| <span data-ttu-id="731e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="731e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="731e8-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="731e8-114">Not Supported</span></span>                               |
| <span data-ttu-id="731e8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="731e8-115">Application</span></span>                            | <span data-ttu-id="731e8-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="731e8-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="731e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="731e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="731e8-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="731e8-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="731e8-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="731e8-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="731e8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="731e8-120">Optional query parameters</span></span>
<span data-ttu-id="731e8-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="731e8-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="731e8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="731e8-122">Request headers</span></span>
| <span data-ttu-id="731e8-123">Имя</span><span class="sxs-lookup"><span data-stu-id="731e8-123">Name</span></span>          | <span data-ttu-id="731e8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="731e8-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="731e8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="731e8-125">Authorization</span></span> | <span data-ttu-id="731e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="731e8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="731e8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="731e8-128">Request body</span></span>
<span data-ttu-id="731e8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="731e8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="731e8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="731e8-130">Response</span></span>
<span data-ttu-id="731e8-131">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект audioRoutingGroup](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="731e8-131">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="731e8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="731e8-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="731e8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="731e8-133">Request</span></span>
<span data-ttu-id="731e8-134">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="731e8-134">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="731e8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="731e8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="731e8-136">C#</span><span class="sxs-lookup"><span data-stu-id="731e8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="731e8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="731e8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="731e8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="731e8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="731e8-139">Java</span><span class="sxs-lookup"><span data-stu-id="731e8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="731e8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="731e8-140">Response</span></span>

> <span data-ttu-id="731e8-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="731e8-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


