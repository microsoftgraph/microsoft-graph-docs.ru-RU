---
title: Создание outlookTaskFolder
description: Создайте папку задачи Outlook в указанном outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3dc2edece1bcb68abb88f1d876782d6ac9e68b80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969522"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="b16c3-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b16c3-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="b16c3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b16c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b16c3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b16c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b16c3-106">Создайте папку задачи Outlook в указанном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="b16c3-106">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b16c3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b16c3-107">Permissions</span></span>
<span data-ttu-id="b16c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b16c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b16c3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b16c3-110">Permission type</span></span>      | <span data-ttu-id="b16c3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b16c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b16c3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b16c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b16c3-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b16c3-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b16c3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b16c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b16c3-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b16c3-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b16c3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b16c3-116">Application</span></span> | <span data-ttu-id="b16c3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b16c3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b16c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b16c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="b16c3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b16c3-119">Request headers</span></span>
| <span data-ttu-id="b16c3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b16c3-120">Name</span></span>       | <span data-ttu-id="b16c3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b16c3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b16c3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b16c3-122">Authorization</span></span>  | <span data-ttu-id="b16c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b16c3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b16c3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b16c3-125">Request body</span></span>
<span data-ttu-id="b16c3-126">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="b16c3-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b16c3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b16c3-127">Response</span></span>

<span data-ttu-id="b16c3-128">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskFolder](../resources/outlooktaskfolder.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b16c3-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b16c3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b16c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b16c3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b16c3-130">Request</span></span>
<span data-ttu-id="b16c3-131">В следующем примере создается задача папку с именем `Cooking` в группе указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="b16c3-131">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
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
<span data-ttu-id="b16c3-132">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="b16c3-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b16c3-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b16c3-133">Response</span></span>
<span data-ttu-id="b16c3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b16c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
