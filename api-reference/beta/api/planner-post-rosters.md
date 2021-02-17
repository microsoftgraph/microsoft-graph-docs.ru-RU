---
title: Создание plannerRoster
description: Создание объекта plannerRoster.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 153a88951943ce1a66d73ee26be289eaae7631f0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272027"
---
# <a name="create-plannerroster"></a><span data-ttu-id="16811-103">Создание plannerRoster</span><span class="sxs-lookup"><span data-stu-id="16811-103">Create plannerRoster</span></span>
<span data-ttu-id="16811-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16811-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16811-105">Создание объекта [plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="16811-105">Create a new [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16811-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16811-106">Permissions</span></span>
<span data-ttu-id="16811-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16811-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16811-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16811-109">Permission type</span></span>|<span data-ttu-id="16811-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16811-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16811-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16811-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16811-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16811-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="16811-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16811-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16811-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16811-114">Not supported.</span></span>|
|<span data-ttu-id="16811-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16811-115">Application</span></span>|<span data-ttu-id="16811-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16811-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16811-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16811-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters
```

## <a name="request-headers"></a><span data-ttu-id="16811-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16811-118">Request headers</span></span>
|<span data-ttu-id="16811-119">Имя</span><span class="sxs-lookup"><span data-stu-id="16811-119">Name</span></span>|<span data-ttu-id="16811-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16811-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16811-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16811-121">Authorization</span></span>|<span data-ttu-id="16811-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16811-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="16811-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16811-124">Content-Type</span></span>|<span data-ttu-id="16811-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16811-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16811-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16811-127">Request body</span></span>
<span data-ttu-id="16811-128">В теле запроса укажу представление объекта [plannerRoster](../resources/plannerroster.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="16811-128">In the request body, supply a JSON representation of the [plannerRoster](../resources/plannerroster.md) object.</span></span>

<span data-ttu-id="16811-129">В [plannerRoster](../resources/plannerroster.md)нет переописаемых свойств.</span><span class="sxs-lookup"><span data-stu-id="16811-129">There are no writable properties on [plannerRoster](../resources/plannerroster.md).</span></span>

## <a name="response"></a><span data-ttu-id="16811-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="16811-130">Response</span></span>

<span data-ttu-id="16811-131">В случае успеха этот метод возвращает код отклика и объект `201 Created` [plannerRoster](../resources/plannerroster.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16811-131">If successful, this method returns a `201 Created` response code and a [plannerRoster](../resources/plannerroster.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16811-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="16811-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16811-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="16811-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="16811-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="16811-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerroster_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters
Content-Type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.plannerRoster"
}
```
# <a name="c"></a>[<span data-ttu-id="16811-135">C#</span><span class="sxs-lookup"><span data-stu-id="16811-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerroster-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16811-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16811-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerroster-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16811-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16811-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerroster-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16811-138">Java</span><span class="sxs-lookup"><span data-stu-id="16811-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerroster-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16811-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="16811-139">Response</span></span>
<span data-ttu-id="16811-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16811-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRoster"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRoster",
  "id": "6519868f-868f-6519-8f86-19658f861965"
}
```

