---
title: Удаление звука группы маршрутизации
description: Удаление указанного audioRoutingGroup.
ms.openlocfilehash: 2683c31f2df4f6913019f6a5f8c58cb009684043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077292"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="548cb-103">Удаление звука группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="548cb-103">Delete audio routing group</span></span>

> <span data-ttu-id="548cb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="548cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="548cb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="548cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="548cb-106">Удаление указанного [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="548cb-106">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="548cb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="548cb-107">Permissions</span></span>
<span data-ttu-id="548cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="548cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="548cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="548cb-110">Permission type</span></span> | <span data-ttu-id="548cb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="548cb-111">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="548cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="548cb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="548cb-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="548cb-113">Not Supported</span></span>        |
| <span data-ttu-id="548cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="548cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="548cb-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="548cb-115">Not Supported</span></span>        |
| <span data-ttu-id="548cb-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="548cb-116">Application</span></span>     | <span data-ttu-id="548cb-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="548cb-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="548cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="548cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="548cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="548cb-119">Request headers</span></span>
| <span data-ttu-id="548cb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="548cb-120">Name</span></span>          | <span data-ttu-id="548cb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="548cb-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="548cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="548cb-122">Authorization</span></span> | <span data-ttu-id="548cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="548cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="548cb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="548cb-125">Request body</span></span>
<span data-ttu-id="548cb-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="548cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="548cb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="548cb-127">Response</span></span>
<span data-ttu-id="548cb-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="548cb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="548cb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="548cb-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="548cb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="548cb-131">Request</span></span>
<span data-ttu-id="548cb-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="548cb-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="548cb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="548cb-133">Response</span></span>

> <span data-ttu-id="548cb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="548cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
