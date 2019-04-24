---
title: Список бесед
description: Получение списка бесед в этой группе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d3f360461d3e943c15c6e7ef39b376a40a601b46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502416"
---
# <a name="list-conversations"></a><span data-ttu-id="f7c77-103">Список бесед</span><span class="sxs-lookup"><span data-stu-id="f7c77-103">List conversations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c77-104">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="f7c77-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c77-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c77-105">Permissions</span></span>
<span data-ttu-id="f7c77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c77-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c77-108">Permission type</span></span>      | <span data-ttu-id="f7c77-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7c77-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7c77-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c77-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7c77-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c77-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c77-113">Not supported.</span></span>    |
|<span data-ttu-id="f7c77-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7c77-114">Application</span></span> | <span data-ttu-id="f7c77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7c77-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7c77-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7c77-117">Optional query parameters</span></span>
<span data-ttu-id="f7c77-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7c77-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7c77-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7c77-119">Request headers</span></span>
| <span data-ttu-id="f7c77-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7c77-120">Header</span></span>       | <span data-ttu-id="f7c77-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f7c77-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7c77-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7c77-122">Authorization</span></span>  | <span data-ttu-id="f7c77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7c77-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7c77-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7c77-125">Request body</span></span>
<span data-ttu-id="f7c77-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7c77-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7c77-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c77-127">Response</span></span>
<span data-ttu-id="f7c77-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c77-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c77-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c77-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7c77-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c77-130">Request</span></span>
<span data-ttu-id="f7c77-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c77-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="f7c77-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c77-132">Response</span></span>
<span data-ttu-id="f7c77-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c77-133">The following is an example of the response.</span></span>
><span data-ttu-id="f7c77-134">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f7c77-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f7c77-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7c77-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-conversations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
