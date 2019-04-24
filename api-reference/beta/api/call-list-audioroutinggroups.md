---
title: Список групп маршрутизации аудио
description: Получение списка объектов **аудиораутингграуп** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a782af2bb7690cc55dd3a4632aeb0cf93734da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461262"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="d4b14-103">Список групп маршрутизации аудио</span><span class="sxs-lookup"><span data-stu-id="d4b14-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4b14-104">Получение списка объектов **аудиораутингграуп** .</span><span class="sxs-lookup"><span data-stu-id="d4b14-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b14-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b14-105">Permissions</span></span>
<span data-ttu-id="d4b14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4b14-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b14-108">Permission type</span></span>                        | <span data-ttu-id="d4b14-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4b14-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4b14-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4b14-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4b14-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4b14-111">Not Supported.</span></span>                               |
| <span data-ttu-id="d4b14-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4b14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4b14-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4b14-113">Not Supported.</span></span>                               |
| <span data-ttu-id="d4b14-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4b14-114">Application</span></span>     | <span data-ttu-id="d4b14-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="d4b14-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4b14-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4b14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4b14-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4b14-117">Optional query parameters</span></span>
<span data-ttu-id="d4b14-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d4b14-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4b14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4b14-119">Request headers</span></span>
| <span data-ttu-id="d4b14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d4b14-120">Name</span></span>          | <span data-ttu-id="d4b14-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d4b14-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d4b14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4b14-122">Authorization</span></span> | <span data-ttu-id="d4b14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4b14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4b14-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4b14-125">Request body</span></span>
<span data-ttu-id="d4b14-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4b14-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b14-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b14-127">Response</span></span>
<span data-ttu-id="d4b14-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4b14-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4b14-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d4b14-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d4b14-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4b14-130">Request</span></span>
<span data-ttu-id="d4b14-131">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4b14-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="d4b14-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4b14-132">Response</span></span>

> <span data-ttu-id="d4b14-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4b14-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
