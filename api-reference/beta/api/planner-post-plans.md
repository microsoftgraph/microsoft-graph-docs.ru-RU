---
title: Создание объекта plannerPlan
description: Используйте этот API, чтобы создать объект **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a77b6861df370995b498448813390c20bf5c7118
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876672"
---
# <a name="create-plannerplan"></a><span data-ttu-id="8a4c0-103">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="8a4c0-103">Create plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a4c0-104">Используйте этот API, чтобы создать объект **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a4c0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a4c0-105">Permissions</span></span>

<span data-ttu-id="8a4c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a4c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a4c0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a4c0-108">Permission type</span></span>                        | <span data-ttu-id="8a4c0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a4c0-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8a4c0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a4c0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a4c0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4c0-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="8a4c0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a4c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4c0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-113">Not supported.</span></span>                              |
| <span data-ttu-id="8a4c0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a4c0-114">Application</span></span>                            | <span data-ttu-id="8a4c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="8a4c0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a4c0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="8a4c0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a4c0-117">Request headers</span></span>

| <span data-ttu-id="8a4c0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8a4c0-118">Name</span></span>          | <span data-ttu-id="8a4c0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8a4c0-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8a4c0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a4c0-120">Authorization</span></span> | <span data-ttu-id="8a4c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a4c0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a4c0-123">Request body</span></span>

<span data-ttu-id="8a4c0-p103">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON. В качестве свойства владельца **PlannerPlan** необходимо указать идентификатор объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="8a4c0-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="8a4c0-126">**Примечание.** Пользователь, создающий план, должен быть участником группы, владеющей планом.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="8a4c0-127">При создании группы с помощью средства [создания группы](../api/group-post-groups.md) вы не становитесь ее участником.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="8a4c0-128">После создания группы добавьте себя в качестве участника с помощью операции [добавления участников группы](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="8a4c0-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="8a4c0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a4c0-129">Response</span></span>

<span data-ttu-id="8a4c0-130">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="8a4c0-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8a4c0-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8a4c0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8a4c0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a4c0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a4c0-135">Request</span></span>

<span data-ttu-id="8a4c0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8a4c0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a4c0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a4c0-138">C#</span><span class="sxs-lookup"><span data-stu-id="8a4c0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a4c0-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="8a4c0-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a4c0-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8a4c0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8a4c0-141">Java</span><span class="sxs-lookup"><span data-stu-id="8a4c0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerplan-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8a4c0-142">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-142">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="8a4c0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a4c0-143">Response</span></span>

<span data-ttu-id="8a4c0-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a4c0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
