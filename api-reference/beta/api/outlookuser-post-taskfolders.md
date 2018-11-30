---
title: Создание outlookTaskFolder
description: Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.
ms.openlocfilehash: 688f3dfb603bec1bc5acb05344e1dc9e8465ae47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079026"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="6ae6c-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="6ae6c-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="6ae6c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ae6c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ae6c-106">Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-106">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ae6c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ae6c-107">Permissions</span></span>
<span data-ttu-id="6ae6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ae6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ae6c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ae6c-110">Permission type</span></span>      | <span data-ttu-id="6ae6c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ae6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ae6c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ae6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ae6c-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ae6c-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="6ae6c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ae6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ae6c-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ae6c-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="6ae6c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ae6c-116">Application</span></span> | <span data-ttu-id="6ae6c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ae6c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ae6c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="6ae6c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ae6c-119">Request headers</span></span>
| <span data-ttu-id="6ae6c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ae6c-120">Name</span></span>       | <span data-ttu-id="6ae6c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6ae6c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ae6c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ae6c-122">Authorization</span></span>  | <span data-ttu-id="6ae6c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ae6c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ae6c-125">Request body</span></span>
<span data-ttu-id="6ae6c-126">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="6ae6c-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6ae6c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ae6c-127">Response</span></span>

<span data-ttu-id="6ae6c-128">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskFolder](../resources/outlooktaskfolder.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ae6c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6ae6c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ae6c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ae6c-130">Request</span></span>
<span data-ttu-id="6ae6c-131">В следующем примере создается задача папку с именем кого в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ae6c-131">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
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
<span data-ttu-id="6ae6c-132">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="6ae6c-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6ae6c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ae6c-133">Response</span></span>
<span data-ttu-id="6ae6c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6ae6c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->