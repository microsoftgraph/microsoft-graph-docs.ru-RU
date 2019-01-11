---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
ms.openlocfilehash: 2640d540c3b5f81c14763f785c565268bb15d689
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851914"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="73b48-103">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="73b48-103">Create outlookTaskGroup</span></span>

> <span data-ttu-id="73b48-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73b48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73b48-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73b48-106">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="73b48-106">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="73b48-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73b48-107">Permissions</span></span>
<span data-ttu-id="73b48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73b48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73b48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73b48-110">Permission type</span></span>      | <span data-ttu-id="73b48-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73b48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73b48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73b48-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73b48-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="73b48-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73b48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b48-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73b48-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="73b48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73b48-116">Application</span></span> | <span data-ttu-id="73b48-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b48-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73b48-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="73b48-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73b48-119">Request headers</span></span>
| <span data-ttu-id="73b48-120">Имя</span><span class="sxs-lookup"><span data-stu-id="73b48-120">Name</span></span>       | <span data-ttu-id="73b48-121">Описание</span><span class="sxs-lookup"><span data-stu-id="73b48-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73b48-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73b48-122">Authorization</span></span>  | <span data-ttu-id="73b48-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73b48-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73b48-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73b48-125">Request body</span></span>
<span data-ttu-id="73b48-126">В тексте запроса укажите представление JSON объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="73b48-126">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="73b48-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="73b48-127">Response</span></span>

<span data-ttu-id="73b48-128">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskGroup](../resources/outlooktaskgroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73b48-128">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b48-129">Пример</span><span class="sxs-lookup"><span data-stu-id="73b48-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73b48-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="73b48-130">Request</span></span>
<span data-ttu-id="73b48-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73b48-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="73b48-132">В тексте запроса укажите представление JSON объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="73b48-132">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="73b48-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="73b48-133">Response</span></span>
<span data-ttu-id="73b48-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="73b48-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
