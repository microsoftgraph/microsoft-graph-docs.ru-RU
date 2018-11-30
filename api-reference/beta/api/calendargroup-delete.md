---
title: Удаление объекта calendarGroup
description: Удаление группы календарей, отличной от стандартной.
ms.openlocfilehash: e71d05a8a0205b10d8735ea0e7baf32f201c7e15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077938"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="5aec3-103">Удаление объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="5aec3-103">Delete calendarGroup</span></span>

> <span data-ttu-id="5aec3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5aec3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5aec3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5aec3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5aec3-106">Удаление группы календарей, отличной от стандартной.</span><span class="sxs-lookup"><span data-stu-id="5aec3-106">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aec3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5aec3-107">Permissions</span></span>

<span data-ttu-id="5aec3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aec3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aec3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5aec3-110">Permission type</span></span>                        | <span data-ttu-id="5aec3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5aec3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5aec3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5aec3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5aec3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aec3-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5aec3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5aec3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aec3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aec3-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5aec3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5aec3-116">Application</span></span>                            | <span data-ttu-id="5aec3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5aec3-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5aec3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5aec3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5aec3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5aec3-119">Request headers</span></span>

| <span data-ttu-id="5aec3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5aec3-120">Name</span></span>          | <span data-ttu-id="5aec3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5aec3-121">Type</span></span>   | <span data-ttu-id="5aec3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5aec3-122">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="5aec3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aec3-123">Authorization</span></span> | <span data-ttu-id="5aec3-124">string</span><span class="sxs-lookup"><span data-stu-id="5aec3-124">string</span></span> | <span data-ttu-id="5aec3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5aec3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aec3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5aec3-127">Request body</span></span>

<span data-ttu-id="5aec3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5aec3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aec3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5aec3-129">Response</span></span>

<span data-ttu-id="5aec3-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5aec3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aec3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5aec3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5aec3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5aec3-133">Request</span></span>

<span data-ttu-id="5aec3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5aec3-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="5aec3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5aec3-135">Response</span></span>

<span data-ttu-id="5aec3-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5aec3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
