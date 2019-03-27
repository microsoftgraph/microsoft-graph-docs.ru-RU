---
title: Получение outlookTaskFolder
description: Получение свойств и связей указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 70ef38ce8b3d808bb66064f69353ef4f2ed0fb5b
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869416"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="88e4e-103">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="88e4e-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88e4e-104">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="88e4e-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="88e4e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88e4e-105">Permissions</span></span>
<span data-ttu-id="88e4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88e4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e4e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88e4e-108">Permission type</span></span>      | <span data-ttu-id="88e4e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88e4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88e4e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88e4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88e4e-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="88e4e-111">Tasks.Read</span></span>    |
|<span data-ttu-id="88e4e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88e4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88e4e-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="88e4e-113">Tasks.Read</span></span>    |
|<span data-ttu-id="88e4e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88e4e-114">Application</span></span> | <span data-ttu-id="88e4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e4e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88e4e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88e4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88e4e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88e4e-117">Optional query parameters</span></span>
<span data-ttu-id="88e4e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="88e4e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88e4e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88e4e-119">Request headers</span></span>
| <span data-ttu-id="88e4e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="88e4e-120">Name</span></span>      |<span data-ttu-id="88e4e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="88e4e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88e4e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88e4e-122">Authorization</span></span>  | <span data-ttu-id="88e4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88e4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88e4e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88e4e-125">Request body</span></span>
<span data-ttu-id="88e4e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88e4e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88e4e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="88e4e-127">Response</span></span>

<span data-ttu-id="88e4e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88e4e-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88e4e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="88e4e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88e4e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="88e4e-130">Request</span></span>
<span data-ttu-id="88e4e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88e4e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAAABrJAAA=')
```
##### <a name="response"></a><span data-ttu-id="88e4e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="88e4e-132">Response</span></span>
<span data-ttu-id="88e4e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88e4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
