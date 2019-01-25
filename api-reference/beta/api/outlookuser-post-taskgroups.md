---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 291eb580228f28754acccff78f60ed6a2004155b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516009"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="c46f7-103">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c46f7-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c46f7-104">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c46f7-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="c46f7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c46f7-105">Permissions</span></span>
<span data-ttu-id="c46f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c46f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c46f7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c46f7-108">Permission type</span></span>      | <span data-ttu-id="c46f7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c46f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c46f7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c46f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c46f7-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c46f7-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c46f7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c46f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c46f7-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c46f7-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c46f7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c46f7-114">Application</span></span> | <span data-ttu-id="c46f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c46f7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c46f7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c46f7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="c46f7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c46f7-117">Request headers</span></span>
| <span data-ttu-id="c46f7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c46f7-118">Name</span></span>       | <span data-ttu-id="c46f7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c46f7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c46f7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c46f7-120">Authorization</span></span>  | <span data-ttu-id="c46f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c46f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c46f7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c46f7-123">Request body</span></span>
<span data-ttu-id="c46f7-124">В тексте запроса укажите представление JSON объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c46f7-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c46f7-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="c46f7-125">Response</span></span>

<span data-ttu-id="c46f7-126">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskGroup](../resources/outlooktaskgroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c46f7-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c46f7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c46f7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c46f7-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c46f7-128">Request</span></span>
<span data-ttu-id="c46f7-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c46f7-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="c46f7-130">В тексте запроса укажите представление JSON объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c46f7-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c46f7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c46f7-131">Response</span></span>
<span data-ttu-id="c46f7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c46f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
