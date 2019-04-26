---
title: Удаление группы маршрутизации звука
description: Удаление указанной группы маршрутизации звука.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c8f61fc536004b841332ecbb398166c26f6541c8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322568"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="b55ca-103">Удаление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="b55ca-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b55ca-104">Удаление указанного [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="b55ca-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b55ca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b55ca-105">Permissions</span></span>
<span data-ttu-id="b55ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b55ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b55ca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b55ca-108">Permission type</span></span> | <span data-ttu-id="b55ca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b55ca-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="b55ca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b55ca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b55ca-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b55ca-111">Not Supported</span></span>        |
| <span data-ttu-id="b55ca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b55ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b55ca-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b55ca-113">Not Supported</span></span>        |
| <span data-ttu-id="b55ca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b55ca-114">Application</span></span>     | <span data-ttu-id="b55ca-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="b55ca-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b55ca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b55ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b55ca-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b55ca-117">Request headers</span></span>
| <span data-ttu-id="b55ca-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b55ca-118">Name</span></span>          | <span data-ttu-id="b55ca-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b55ca-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b55ca-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b55ca-120">Authorization</span></span> | <span data-ttu-id="b55ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b55ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b55ca-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b55ca-123">Request body</span></span>
<span data-ttu-id="b55ca-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b55ca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b55ca-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b55ca-125">Response</span></span>
<span data-ttu-id="b55ca-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b55ca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b55ca-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b55ca-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b55ca-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b55ca-129">Request</span></span>
<span data-ttu-id="b55ca-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b55ca-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="b55ca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b55ca-131">Response</span></span>

> <span data-ttu-id="b55ca-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b55ca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
