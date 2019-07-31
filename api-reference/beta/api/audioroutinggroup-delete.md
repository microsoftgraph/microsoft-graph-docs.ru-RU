---
title: Удаление группы маршрутизации звука
description: Удаление указанной группы маршрутизации звука.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aabc4337e4c48d4e4c2b86824f9d2448c9cf805f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945342"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="7e9b5-103">Удаление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="7e9b5-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e9b5-104">Удаление указанного [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="7e9b5-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e9b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e9b5-105">Permissions</span></span>
<span data-ttu-id="7e9b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e9b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e9b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e9b5-108">Permission type</span></span> | <span data-ttu-id="7e9b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e9b5-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="7e9b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e9b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e9b5-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7e9b5-111">Not Supported</span></span>        |
| <span data-ttu-id="7e9b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e9b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e9b5-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7e9b5-113">Not Supported</span></span>        |
| <span data-ttu-id="7e9b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e9b5-114">Application</span></span>     | <span data-ttu-id="7e9b5-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="7e9b5-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e9b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e9b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e9b5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e9b5-117">Request headers</span></span>
| <span data-ttu-id="7e9b5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e9b5-118">Name</span></span>          | <span data-ttu-id="7e9b5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e9b5-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7e9b5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e9b5-120">Authorization</span></span> | <span data-ttu-id="7e9b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e9b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e9b5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e9b5-123">Request body</span></span>
<span data-ttu-id="7e9b5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e9b5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e9b5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e9b5-125">Response</span></span>
<span data-ttu-id="7e9b5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7e9b5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e9b5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7e9b5-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e9b5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e9b5-129">Request</span></span>
<span data-ttu-id="7e9b5-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e9b5-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e9b5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9b5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e9b5-132">C#</span><span class="sxs-lookup"><span data-stu-id="7e9b5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e9b5-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e9b5-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e9b5-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7e9b5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e9b5-135">Java</span><span class="sxs-lookup"><span data-stu-id="7e9b5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e9b5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e9b5-136">Response</span></span>

> <span data-ttu-id="7e9b5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e9b5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
