---
title: Удаление plannerRoster
description: Удаляет объект plannerRoster.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e6159e9a5f4a230e3bb60f04fca6abdee1ee3a97
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271936"
---
# <a name="delete-plannerroster"></a><span data-ttu-id="99602-103">Удаление plannerRoster</span><span class="sxs-lookup"><span data-stu-id="99602-103">Delete plannerRoster</span></span>
<span data-ttu-id="99602-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99602-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99602-105">Удаление объекта [plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="99602-105">Delete a [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99602-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99602-106">Permissions</span></span>
<span data-ttu-id="99602-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99602-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99602-109">Permission type</span></span>|<span data-ttu-id="99602-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99602-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99602-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99602-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99602-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99602-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="99602-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99602-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99602-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99602-114">Not supported.</span></span>|
|<span data-ttu-id="99602-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99602-115">Application</span></span>|<span data-ttu-id="99602-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99602-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99602-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99602-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /planner/rosters/{plannerRosterId}
```

## <a name="request-headers"></a><span data-ttu-id="99602-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99602-118">Request headers</span></span>
|<span data-ttu-id="99602-119">Имя</span><span class="sxs-lookup"><span data-stu-id="99602-119">Name</span></span>|<span data-ttu-id="99602-120">Описание</span><span class="sxs-lookup"><span data-stu-id="99602-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="99602-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99602-121">Authorization</span></span>|<span data-ttu-id="99602-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99602-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99602-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99602-124">Request body</span></span>
<span data-ttu-id="99602-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99602-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99602-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="99602-126">Response</span></span>

<span data-ttu-id="99602-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="99602-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="99602-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="99602-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99602-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="99602-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="99602-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="99602-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerroster"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38
```
# <a name="c"></a>[<span data-ttu-id="99602-131">C#</span><span class="sxs-lookup"><span data-stu-id="99602-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerroster-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99602-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99602-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerroster-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99602-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99602-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerroster-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99602-134">Java</span><span class="sxs-lookup"><span data-stu-id="99602-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerroster-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="99602-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="99602-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

