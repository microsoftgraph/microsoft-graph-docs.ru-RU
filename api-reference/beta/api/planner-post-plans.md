---
title: Создание объекта plannerPlan
description: Используйте этот API, чтобы создать объект **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a5383bacedef2e7e6df718a4286f034e67f6a7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524718"
---
# <a name="create-plannerplan"></a><span data-ttu-id="f9ecb-103">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f9ecb-103">Create plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ecb-104">Используйте этот API, чтобы создать объект **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9ecb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ecb-105">Permissions</span></span>

<span data-ttu-id="f9ecb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9ecb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ecb-108">Permission type</span></span>                        | <span data-ttu-id="f9ecb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9ecb-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f9ecb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9ecb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9ecb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ecb-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="f9ecb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9ecb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ecb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-113">Not supported.</span></span>                              |
| <span data-ttu-id="f9ecb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9ecb-114">Application</span></span>                            | <span data-ttu-id="f9ecb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="f9ecb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9ecb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="f9ecb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9ecb-117">Request headers</span></span>

| <span data-ttu-id="f9ecb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f9ecb-118">Name</span></span>          | <span data-ttu-id="f9ecb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f9ecb-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f9ecb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9ecb-120">Authorization</span></span> | <span data-ttu-id="f9ecb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9ecb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9ecb-123">Request body</span></span>

<span data-ttu-id="f9ecb-p103">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON. В качестве свойства владельца **PlannerPlan** необходимо указать идентификатор объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="f9ecb-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="f9ecb-126">**Примечание:** Пользователя, создающего план должен быть членом группы, который будет владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="f9ecb-127">При создании новой группы с помощью [Создать группу](../api/group-post-groups.md), вы не добавляются в группу как члена группы.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="f9ecb-128">После создания группы добавьте себя в качестве члена с помощью [учета членов группы](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="f9ecb-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="f9ecb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ecb-129">Response</span></span>

<span data-ttu-id="f9ecb-130">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="f9ecb-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f9ecb-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f9ecb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f9ecb-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9ecb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9ecb-135">Request</span></span>

<span data-ttu-id="f9ecb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-136">Here is an example of the request.</span></span>
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

<span data-ttu-id="f9ecb-137">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9ecb-137">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="f9ecb-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9ecb-138">Response</span></span>

<span data-ttu-id="f9ecb-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f9ecb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/planner-post-plans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
