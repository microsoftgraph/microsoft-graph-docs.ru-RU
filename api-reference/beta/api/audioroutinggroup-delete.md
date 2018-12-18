---
title: Удаление звука группы маршрутизации
description: Удаление указанного audioRoutingGroup.
author: VinodRavichandran
ms.openlocfilehash: 025498e1ceb6178ede4c7ca938c7b0d3d05a80ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323942"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="abc37-103">Удаление звука группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="abc37-103">Delete audio routing group</span></span>

> <span data-ttu-id="abc37-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abc37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abc37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abc37-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abc37-106">Удаление указанного [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="abc37-106">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="abc37-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abc37-107">Permissions</span></span>
<span data-ttu-id="abc37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="abc37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abc37-110">Permission type</span></span> | <span data-ttu-id="abc37-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abc37-111">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="abc37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abc37-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="abc37-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="abc37-113">Not Supported</span></span>        |
| <span data-ttu-id="abc37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abc37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abc37-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="abc37-115">Not Supported</span></span>        |
| <span data-ttu-id="abc37-116">Application</span><span class="sxs-lookup"><span data-stu-id="abc37-116">Application</span></span>     | <span data-ttu-id="abc37-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="abc37-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abc37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abc37-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="abc37-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abc37-119">Request headers</span></span>
| <span data-ttu-id="abc37-120">Имя</span><span class="sxs-lookup"><span data-stu-id="abc37-120">Name</span></span>          | <span data-ttu-id="abc37-121">Описание</span><span class="sxs-lookup"><span data-stu-id="abc37-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="abc37-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abc37-122">Authorization</span></span> | <span data-ttu-id="abc37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abc37-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abc37-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abc37-125">Request body</span></span>
<span data-ttu-id="abc37-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abc37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abc37-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="abc37-127">Response</span></span>
<span data-ttu-id="abc37-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="abc37-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abc37-130">Пример</span><span class="sxs-lookup"><span data-stu-id="abc37-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="abc37-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="abc37-131">Request</span></span>
<span data-ttu-id="abc37-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abc37-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="abc37-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="abc37-133">Response</span></span>

> <span data-ttu-id="abc37-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abc37-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
