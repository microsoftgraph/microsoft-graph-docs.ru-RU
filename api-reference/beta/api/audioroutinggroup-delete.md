---
title: Удаление группы маршрутизации звука
description: Удаление указанной группы маршрутизации звука.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4144a1701d7fe96d507911ebed0ca36e242ac47
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636473"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="b8434-103">Удаление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="b8434-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8434-104">Удаление указанного [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="b8434-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8434-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8434-105">Permissions</span></span>
<span data-ttu-id="b8434-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8434-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8434-108">Permission type</span></span> | <span data-ttu-id="b8434-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8434-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="b8434-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8434-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8434-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b8434-111">Not Supported</span></span>        |
| <span data-ttu-id="b8434-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8434-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8434-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b8434-113">Not Supported</span></span>        |
| <span data-ttu-id="b8434-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8434-114">Application</span></span>     | <span data-ttu-id="b8434-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="b8434-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8434-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8434-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8434-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8434-117">Request headers</span></span>
| <span data-ttu-id="b8434-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b8434-118">Name</span></span>          | <span data-ttu-id="b8434-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b8434-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b8434-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8434-120">Authorization</span></span> | <span data-ttu-id="b8434-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8434-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8434-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8434-123">Request body</span></span>
<span data-ttu-id="b8434-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8434-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8434-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8434-125">Response</span></span>
<span data-ttu-id="b8434-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b8434-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8434-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b8434-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8434-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8434-129">Request</span></span>
<span data-ttu-id="b8434-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8434-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="b8434-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8434-131">Response</span></span>

> <span data-ttu-id="b8434-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8434-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b8434-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b8434-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b8434-135">Языках</span><span class="sxs-lookup"><span data-stu-id="b8434-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8434-136">Язык</span><span class="sxs-lookup"><span data-stu-id="b8434-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
