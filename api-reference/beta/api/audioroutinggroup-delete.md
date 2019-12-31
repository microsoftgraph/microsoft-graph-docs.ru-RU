---
title: Удаление группы маршрутизации звука
description: Удаление указанной группы маршрутизации звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7f89c223c7e45ccaa5a25fe7bbdd7a53f529880f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911848"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="d89f6-103">Удаление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="d89f6-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d89f6-104">Удаление указанного [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="d89f6-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d89f6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d89f6-105">Permissions</span></span>
<span data-ttu-id="d89f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d89f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d89f6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d89f6-108">Permission type</span></span> | <span data-ttu-id="d89f6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d89f6-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="d89f6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d89f6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d89f6-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d89f6-111">Not Supported</span></span>        |
| <span data-ttu-id="d89f6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d89f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d89f6-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d89f6-113">Not Supported</span></span>        |
| <span data-ttu-id="d89f6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d89f6-114">Application</span></span>     | <span data-ttu-id="d89f6-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="d89f6-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d89f6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d89f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="d89f6-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d89f6-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d89f6-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d89f6-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d89f6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d89f6-119">Request headers</span></span>
| <span data-ttu-id="d89f6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d89f6-120">Name</span></span>          | <span data-ttu-id="d89f6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d89f6-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d89f6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d89f6-122">Authorization</span></span> | <span data-ttu-id="d89f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d89f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d89f6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d89f6-125">Request body</span></span>
<span data-ttu-id="d89f6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d89f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d89f6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="d89f6-127">Response</span></span>
<span data-ttu-id="d89f6-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d89f6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d89f6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d89f6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d89f6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d89f6-131">Request</span></span>
<span data-ttu-id="d89f6-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d89f6-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d89f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d89f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d89f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="d89f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d89f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d89f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d89f6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d89f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d89f6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d89f6-137">Response</span></span>

> <span data-ttu-id="d89f6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d89f6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
