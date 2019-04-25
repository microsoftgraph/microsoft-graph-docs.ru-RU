---
title: Создание outlookTaskFolder
description: Создайте папку задач Outlook в заданном outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d1c6621e16d548b24cba264cb0434c5ea5dbd290
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539645"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="ce37c-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ce37c-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce37c-104">Создайте папку задач Outlook в заданном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="ce37c-104">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ce37c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce37c-105">Permissions</span></span>
<span data-ttu-id="ce37c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce37c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce37c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce37c-108">Permission type</span></span>      | <span data-ttu-id="ce37c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce37c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce37c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce37c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce37c-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce37c-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ce37c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce37c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce37c-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce37c-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ce37c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce37c-114">Application</span></span> | <span data-ttu-id="ce37c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce37c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce37c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce37c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="ce37c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce37c-117">Request headers</span></span>
| <span data-ttu-id="ce37c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ce37c-118">Name</span></span>       | <span data-ttu-id="ce37c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ce37c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ce37c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce37c-120">Authorization</span></span>  | <span data-ttu-id="ce37c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce37c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce37c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce37c-123">Request body</span></span>
<span data-ttu-id="ce37c-124">В тексте запроса добавьте представление объекта [OutlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce37c-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ce37c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce37c-125">Response</span></span>

<span data-ttu-id="ce37c-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce37c-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce37c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ce37c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce37c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce37c-128">Request</span></span>
<span data-ttu-id="ce37c-129">В следующем примере создается папка задач, вызываемая `Cooking` из указанной группы задач.</span><span class="sxs-lookup"><span data-stu-id="ce37c-129">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups('AAMkADIyAAAhrbe-AAA')/taskfolders 

Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
<span data-ttu-id="ce37c-130">В тексте запроса добавьте представление объекта [OutlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce37c-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ce37c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce37c-131">Response</span></span>
<span data-ttu-id="ce37c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce37c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
