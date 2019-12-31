---
title: Список групп маршрутизации аудио
description: Получение списка объектов **аудиораутингграуп** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 04b46d8476768b2a39b86e9803d778dafee3e0f3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912764"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="614dd-103">Список групп маршрутизации аудио</span><span class="sxs-lookup"><span data-stu-id="614dd-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="614dd-104">Получение списка объектов **аудиораутингграуп** .</span><span class="sxs-lookup"><span data-stu-id="614dd-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="614dd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="614dd-105">Permissions</span></span>
<span data-ttu-id="614dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="614dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="614dd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="614dd-108">Permission type</span></span>                        | <span data-ttu-id="614dd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="614dd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="614dd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="614dd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="614dd-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="614dd-111">Not Supported.</span></span>                               |
| <span data-ttu-id="614dd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="614dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="614dd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="614dd-113">Not Supported.</span></span>                               |
| <span data-ttu-id="614dd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="614dd-114">Application</span></span>     | <span data-ttu-id="614dd-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="614dd-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="614dd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="614dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="614dd-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="614dd-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="614dd-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="614dd-118">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="614dd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="614dd-119">Optional query parameters</span></span>
<span data-ttu-id="614dd-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="614dd-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="614dd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="614dd-121">Request headers</span></span>
| <span data-ttu-id="614dd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="614dd-122">Name</span></span>          | <span data-ttu-id="614dd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="614dd-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="614dd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="614dd-124">Authorization</span></span> | <span data-ttu-id="614dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="614dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="614dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="614dd-127">Request body</span></span>
<span data-ttu-id="614dd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="614dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="614dd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="614dd-129">Response</span></span>
<span data-ttu-id="614dd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="614dd-130">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="614dd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="614dd-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="614dd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="614dd-132">Request</span></span>
<span data-ttu-id="614dd-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="614dd-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="614dd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="614dd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="614dd-135">C#</span><span class="sxs-lookup"><span data-stu-id="614dd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="614dd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="614dd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="614dd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="614dd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="614dd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="614dd-138">Response</span></span>

> <span data-ttu-id="614dd-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="614dd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
