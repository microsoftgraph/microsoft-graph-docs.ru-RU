---
title: Удаление группы маршрутизации звука
description: Удалите указанную группу маршрутов аудио.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: de1ac6aa2a296cf95fddb33c075f52ce57da0d81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048024"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="8f14a-103">Удаление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="8f14a-103">Delete audio routing group</span></span>

<span data-ttu-id="8f14a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f14a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f14a-105">Удаление указанной [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="8f14a-105">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f14a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f14a-106">Permissions</span></span>
<span data-ttu-id="8f14a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f14a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f14a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f14a-109">Permission type</span></span> | <span data-ttu-id="8f14a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f14a-110">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="8f14a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f14a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f14a-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f14a-112">Not Supported</span></span>        |
| <span data-ttu-id="8f14a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f14a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f14a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f14a-114">Not Supported</span></span>        |
| <span data-ttu-id="8f14a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f14a-115">Application</span></span>     | <span data-ttu-id="8f14a-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="8f14a-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f14a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f14a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="8f14a-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8f14a-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8f14a-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="8f14a-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f14a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f14a-120">Request headers</span></span>
| <span data-ttu-id="8f14a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8f14a-121">Name</span></span>          | <span data-ttu-id="8f14a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8f14a-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8f14a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f14a-123">Authorization</span></span> | <span data-ttu-id="8f14a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f14a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f14a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f14a-126">Request body</span></span>
<span data-ttu-id="8f14a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f14a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f14a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f14a-128">Response</span></span>
<span data-ttu-id="8f14a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8f14a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f14a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f14a-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f14a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f14a-132">Request</span></span>
<span data-ttu-id="8f14a-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f14a-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f14a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f14a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="8f14a-135">C#</span><span class="sxs-lookup"><span data-stu-id="8f14a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f14a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f14a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f14a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f14a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f14a-138">Java</span><span class="sxs-lookup"><span data-stu-id="8f14a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f14a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f14a-139">Response</span></span>

> <span data-ttu-id="8f14a-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8f14a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "suppressions": [
  ]
}
-->


