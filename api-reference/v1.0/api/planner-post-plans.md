---
title: Создание объекта plannerPlan
description: Используйте этот API, чтобы создать объект **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1bb26d2858cf3b37ca6d61095eedca5ec8a4294d
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473635"
---
# <a name="create-plannerplan"></a><span data-ttu-id="3cb0e-103">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3cb0e-103">Create plannerPlan</span></span>

<span data-ttu-id="3cb0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cb0e-105">Используйте этот API, чтобы создать объект **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-105">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb0e-106">Permissions</span></span>

<span data-ttu-id="3cb0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cb0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb0e-109">Permission type</span></span>                        | <span data-ttu-id="3cb0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cb0e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3cb0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cb0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cb0e-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb0e-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="3cb0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cb0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cb0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-114">Not supported.</span></span>                              |
| <span data-ttu-id="3cb0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cb0e-115">Application</span></span>                            | <span data-ttu-id="3cb0e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3cb0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cb0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="3cb0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cb0e-118">Request headers</span></span>

| <span data-ttu-id="3cb0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3cb0e-119">Name</span></span>          | <span data-ttu-id="3cb0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb0e-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3cb0e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cb0e-121">Authorization</span></span> | <span data-ttu-id="3cb0e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cb0e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cb0e-124">Request body</span></span>

<span data-ttu-id="3cb0e-p103">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON. В качестве свойства владельца **PlannerPlan** необходимо указать идентификатор объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="3cb0e-127">**Примечание.** Пользователь, создающий план, должен быть участником группы, владеющей планом.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-127">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="3cb0e-128">При создании группы с помощью средства [создания группы](../api/group-post-groups.md) вы не становитесь ее участником.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-128">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="3cb0e-129">После создания группы добавьте себя в качестве участника с помощью операции [добавления участников группы](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="3cb0e-129">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="3cb0e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb0e-130">Response</span></span>

<span data-ttu-id="3cb0e-131">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-131">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="3cb0e-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3cb0e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3cb0e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cb0e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cb0e-136">Request</span></span>

<span data-ttu-id="3cb0e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cb0e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb0e-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3cb0e-139">C#</span><span class="sxs-lookup"><span data-stu-id="3cb0e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cb0e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cb0e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cb0e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cb0e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cb0e-142">Java</span><span class="sxs-lookup"><span data-stu-id="3cb0e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerplan-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3cb0e-143">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-143">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="3cb0e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb0e-144">Response</span></span>

<span data-ttu-id="3cb0e-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

