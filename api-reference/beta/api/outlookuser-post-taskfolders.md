---
title: Создание outlookTaskFolder
description: Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 81c77d96b4d7c66cfbc7dde3481a7bfaa8cd6c5f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514448"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="de6ac-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="de6ac-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6ac-104">Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="de6ac-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="de6ac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de6ac-105">Permissions</span></span>
<span data-ttu-id="de6ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6ac-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de6ac-108">Permission type</span></span>      | <span data-ttu-id="de6ac-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de6ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6ac-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de6ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de6ac-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6ac-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="de6ac-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de6ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6ac-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6ac-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="de6ac-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de6ac-114">Application</span></span> | <span data-ttu-id="de6ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6ac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de6ac-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de6ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="de6ac-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de6ac-117">Request headers</span></span>
| <span data-ttu-id="de6ac-118">Имя</span><span class="sxs-lookup"><span data-stu-id="de6ac-118">Name</span></span>       | <span data-ttu-id="de6ac-119">Описание</span><span class="sxs-lookup"><span data-stu-id="de6ac-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de6ac-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de6ac-120">Authorization</span></span>  | <span data-ttu-id="de6ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de6ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de6ac-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de6ac-123">Request body</span></span>
<span data-ttu-id="de6ac-124">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="de6ac-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de6ac-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="de6ac-125">Response</span></span>

<span data-ttu-id="de6ac-126">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskFolder](../resources/outlooktaskfolder.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="de6ac-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de6ac-127">Пример</span><span class="sxs-lookup"><span data-stu-id="de6ac-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de6ac-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="de6ac-128">Request</span></span>
<span data-ttu-id="de6ac-129">В следующем примере создается задача папку с именем кого в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="de6ac-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
<span data-ttu-id="de6ac-130">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="de6ac-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="de6ac-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="de6ac-131">Response</span></span>
<span data-ttu-id="de6ac-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="de6ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
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
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
