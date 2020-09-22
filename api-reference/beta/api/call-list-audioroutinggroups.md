---
title: Список групп маршрутизации аудио
description: Получение списка объектов **аудиораутингграуп** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b1b229316370488a441ad4bacee8b92af42951c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987395"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="49638-103">Список групп маршрутизации аудио</span><span class="sxs-lookup"><span data-stu-id="49638-103">List audio routing groups</span></span>

<span data-ttu-id="49638-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49638-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49638-105">Получение списка объектов **аудиораутингграуп** .</span><span class="sxs-lookup"><span data-stu-id="49638-105">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="49638-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49638-106">Permissions</span></span>
<span data-ttu-id="49638-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49638-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49638-109">Permission type</span></span>                        | <span data-ttu-id="49638-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49638-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49638-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49638-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49638-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49638-112">Not Supported.</span></span>                               |
| <span data-ttu-id="49638-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49638-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49638-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49638-114">Not Supported.</span></span>                               |
| <span data-ttu-id="49638-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49638-115">Application</span></span>     | <span data-ttu-id="49638-116">Calls. Жоинграупкаллс. ALL, Calls.IniТиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="49638-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49638-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49638-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="49638-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="49638-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="49638-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="49638-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="49638-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49638-120">Optional query parameters</span></span>
<span data-ttu-id="49638-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49638-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49638-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49638-122">Request headers</span></span>
| <span data-ttu-id="49638-123">Имя</span><span class="sxs-lookup"><span data-stu-id="49638-123">Name</span></span>          | <span data-ttu-id="49638-124">Описание</span><span class="sxs-lookup"><span data-stu-id="49638-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="49638-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49638-125">Authorization</span></span> | <span data-ttu-id="49638-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49638-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49638-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49638-128">Request body</span></span>
<span data-ttu-id="49638-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49638-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49638-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="49638-130">Response</span></span>
<span data-ttu-id="49638-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49638-131">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49638-132">Пример</span><span class="sxs-lookup"><span data-stu-id="49638-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="49638-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="49638-133">Request</span></span>
<span data-ttu-id="49638-134">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49638-134">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="49638-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="49638-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
```
# <a name="c"></a>[<span data-ttu-id="49638-136">C#</span><span class="sxs-lookup"><span data-stu-id="49638-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49638-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49638-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49638-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49638-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49638-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="49638-139">Response</span></span>

> <span data-ttu-id="49638-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49638-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


