---
title: Список taskFolders
description: Получение папки задач Outlook в определенных outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 16a3463a7cdc4a3bc4efd401c7ca1a8932c82b7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508288"
---
# <a name="list-taskfolders"></a><span data-ttu-id="bcf99-103">Список taskFolders</span><span class="sxs-lookup"><span data-stu-id="bcf99-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf99-104">Получение папки задач Outlook в определенных [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="bcf99-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bcf99-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf99-105">Permissions</span></span>
<span data-ttu-id="bcf99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf99-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf99-108">Permission type</span></span>      | <span data-ttu-id="bcf99-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcf99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcf99-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcf99-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcf99-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bcf99-111">Tasks.Read</span></span>    |
|<span data-ttu-id="bcf99-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcf99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcf99-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bcf99-113">Tasks.Read</span></span>    |
|<span data-ttu-id="bcf99-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcf99-114">Application</span></span> | <span data-ttu-id="bcf99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf99-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcf99-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcf99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bcf99-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bcf99-117">Optional query parameters</span></span>
<span data-ttu-id="bcf99-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bcf99-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcf99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcf99-119">Request headers</span></span>
| <span data-ttu-id="bcf99-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bcf99-120">Name</span></span>      |<span data-ttu-id="bcf99-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf99-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bcf99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcf99-122">Authorization</span></span>  | <span data-ttu-id="bcf99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcf99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcf99-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcf99-125">Request body</span></span>
<span data-ttu-id="bcf99-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcf99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcf99-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcf99-127">Response</span></span>

<span data-ttu-id="bcf99-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTaskFolder](../resources/outlooktaskfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bcf99-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bcf99-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bcf99-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcf99-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcf99-130">Request</span></span>
<span data-ttu-id="bcf99-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcf99-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="bcf99-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcf99-132">Response</span></span>
<span data-ttu-id="bcf99-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bcf99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
    {
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-list-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
