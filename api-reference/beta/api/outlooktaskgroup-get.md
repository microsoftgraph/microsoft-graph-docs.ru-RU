---
title: Получение outlookTaskGroup
description: Получение свойств и связей указанной группы задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b4f260d1ae19cca26720a59f68125caac3b5a846
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539868"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="a1ecb-103">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a1ecb-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1ecb-104">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1ecb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1ecb-105">Permissions</span></span>
<span data-ttu-id="a1ecb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1ecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1ecb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1ecb-108">Permission type</span></span>      | <span data-ttu-id="a1ecb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1ecb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1ecb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1ecb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a1ecb-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a1ecb-111">Tasks.Read</span></span>    |
|<span data-ttu-id="a1ecb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1ecb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1ecb-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a1ecb-113">Tasks.Read</span></span>    |
|<span data-ttu-id="a1ecb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1ecb-114">Application</span></span> | <span data-ttu-id="a1ecb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1ecb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1ecb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1ecb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1ecb-117">Optional query parameters</span></span>
<span data-ttu-id="a1ecb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1ecb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1ecb-119">Request headers</span></span>
| <span data-ttu-id="a1ecb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a1ecb-120">Name</span></span>      |<span data-ttu-id="a1ecb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ecb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1ecb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1ecb-122">Authorization</span></span>  | <span data-ttu-id="a1ecb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1ecb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1ecb-125">Request body</span></span>
<span data-ttu-id="a1ecb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1ecb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1ecb-127">Response</span></span>

<span data-ttu-id="a1ecb-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1ecb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a1ecb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1ecb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1ecb-130">Request</span></span>
<span data-ttu-id="a1ecb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="a1ecb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1ecb-132">Response</span></span>
<span data-ttu-id="a1ecb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1ecb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
