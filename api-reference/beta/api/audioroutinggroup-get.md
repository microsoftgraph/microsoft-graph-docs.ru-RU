---
title: Получение группы маршрутизации звука
description: Получение свойств и связей объекта Аудиораутингграуп.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0a93108e557804a4d6c1ad5b1da608a51cbc7d07
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911778"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="06fff-103">Получение группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="06fff-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06fff-104">Получение свойств и связей объекта [аудиораутингграуп](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="06fff-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="06fff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06fff-105">Permissions</span></span>
<span data-ttu-id="06fff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06fff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06fff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06fff-108">Permission type</span></span>                        | <span data-ttu-id="06fff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06fff-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06fff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06fff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="06fff-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="06fff-111">Not Supported</span></span>                               |
| <span data-ttu-id="06fff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06fff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06fff-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="06fff-113">Not Supported</span></span>                               |
| <span data-ttu-id="06fff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06fff-114">Application</span></span>                            | <span data-ttu-id="06fff-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="06fff-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06fff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06fff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="06fff-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="06fff-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="06fff-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="06fff-118">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="06fff-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06fff-119">Optional query parameters</span></span>
<span data-ttu-id="06fff-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="06fff-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06fff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06fff-121">Request headers</span></span>
| <span data-ttu-id="06fff-122">Имя</span><span class="sxs-lookup"><span data-stu-id="06fff-122">Name</span></span>          | <span data-ttu-id="06fff-123">Описание</span><span class="sxs-lookup"><span data-stu-id="06fff-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="06fff-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06fff-124">Authorization</span></span> | <span data-ttu-id="06fff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06fff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06fff-127">Request body</span></span>
<span data-ttu-id="06fff-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06fff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06fff-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="06fff-129">Response</span></span>
<span data-ttu-id="06fff-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06fff-130">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06fff-131">Пример</span><span class="sxs-lookup"><span data-stu-id="06fff-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="06fff-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06fff-132">Request</span></span>
<span data-ttu-id="06fff-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06fff-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="06fff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="06fff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06fff-135">C#</span><span class="sxs-lookup"><span data-stu-id="06fff-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06fff-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06fff-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06fff-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06fff-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="06fff-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="06fff-138">Response</span></span>

> <span data-ttu-id="06fff-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06fff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
