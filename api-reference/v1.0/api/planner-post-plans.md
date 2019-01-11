---
title: Создание объекта plannerPlan
description: Используйте этот API, чтобы создать объект **plannerPlan**.
localization_priority: Normal
ms.openlocfilehash: 4a896ab44e0e66ae81f3cfa43ac73ecbc5209acc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871668"
---
# <a name="create-plannerplan"></a><span data-ttu-id="e60f5-103">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e60f5-103">Create plannerPlan</span></span>

<span data-ttu-id="e60f5-104">Используйте этот API, чтобы создать объект **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="e60f5-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e60f5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e60f5-105">Permissions</span></span>

<span data-ttu-id="e60f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e60f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e60f5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e60f5-108">Permission type</span></span>                        | <span data-ttu-id="e60f5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e60f5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e60f5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e60f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e60f5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e60f5-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="e60f5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e60f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e60f5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e60f5-113">Not supported.</span></span>                              |
| <span data-ttu-id="e60f5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e60f5-114">Application</span></span>                            | <span data-ttu-id="e60f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e60f5-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="e60f5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e60f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="e60f5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e60f5-117">Request headers</span></span>

| <span data-ttu-id="e60f5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e60f5-118">Name</span></span>          | <span data-ttu-id="e60f5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e60f5-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e60f5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e60f5-120">Authorization</span></span> | <span data-ttu-id="e60f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e60f5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e60f5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e60f5-123">Request body</span></span>

<span data-ttu-id="e60f5-p103">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON. В качестве свойства владельца **PlannerPlan** необходимо указать идентификатор объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="e60f5-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="e60f5-126">**Примечание:** Пользователя, создающего план должен быть членом группы, который будет владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="e60f5-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="e60f5-127">При создании новой группы с помощью [Создать группу](../api/group-post-groups.md), вы не добавляются в группу как члена группы.</span><span class="sxs-lookup"><span data-stu-id="e60f5-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="e60f5-128">После создания группы добавьте себя в качестве члена с помощью [учета членов группы](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="e60f5-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="e60f5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e60f5-129">Response</span></span>

<span data-ttu-id="e60f5-130">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e60f5-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="e60f5-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e60f5-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e60f5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e60f5-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e60f5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e60f5-135">Request</span></span>

<span data-ttu-id="e60f5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e60f5-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```

<span data-ttu-id="e60f5-137">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e60f5-137">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="e60f5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e60f5-138">Response</span></span>

<span data-ttu-id="e60f5-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e60f5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
