---
title: Удаление группы маршрутизации звука
description: Удаление указанной группы маршрутизации звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 87cada1f74e36398fef2f1eda82d622540c7ac47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991722"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="14d95-103">Удаление группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="14d95-103">Delete audio routing group</span></span>

<span data-ttu-id="14d95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14d95-105">Удаление указанного [аудиораутингграуп](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="14d95-105">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="14d95-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14d95-106">Permissions</span></span>
<span data-ttu-id="14d95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14d95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14d95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14d95-109">Permission type</span></span> | <span data-ttu-id="14d95-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14d95-110">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="14d95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14d95-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14d95-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="14d95-112">Not Supported</span></span>        |
| <span data-ttu-id="14d95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14d95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14d95-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="14d95-114">Not Supported</span></span>        |
| <span data-ttu-id="14d95-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14d95-115">Application</span></span>     | <span data-ttu-id="14d95-116">Calls. Жоинграупкаллс. ALL, Calls.IniТиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="14d95-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14d95-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14d95-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="14d95-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="14d95-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="14d95-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="14d95-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14d95-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14d95-120">Request headers</span></span>
| <span data-ttu-id="14d95-121">Имя</span><span class="sxs-lookup"><span data-stu-id="14d95-121">Name</span></span>          | <span data-ttu-id="14d95-122">Описание</span><span class="sxs-lookup"><span data-stu-id="14d95-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="14d95-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14d95-123">Authorization</span></span> | <span data-ttu-id="14d95-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14d95-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14d95-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14d95-126">Request body</span></span>
<span data-ttu-id="14d95-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14d95-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14d95-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="14d95-128">Response</span></span>
<span data-ttu-id="14d95-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="14d95-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d95-131">Пример</span><span class="sxs-lookup"><span data-stu-id="14d95-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="14d95-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="14d95-132">Request</span></span>
<span data-ttu-id="14d95-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14d95-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14d95-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="14d95-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="14d95-135">C#</span><span class="sxs-lookup"><span data-stu-id="14d95-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14d95-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14d95-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14d95-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14d95-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="14d95-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="14d95-138">Response</span></span>

> <span data-ttu-id="14d95-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14d95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


