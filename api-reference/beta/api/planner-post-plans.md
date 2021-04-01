---
title: Создание объекта plannerPlan
description: Используйте этот API, чтобы создать объект **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a12e055c4972f7064cdf91239502b7bb54e5c787
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473817"
---
# <a name="create-plannerplan"></a><span data-ttu-id="4e00b-103">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="4e00b-103">Create plannerPlan</span></span>

<span data-ttu-id="4e00b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e00b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e00b-105">Создание нового **планировщикаPlan**.</span><span class="sxs-lookup"><span data-stu-id="4e00b-105">Create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e00b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e00b-106">Permissions</span></span>

<span data-ttu-id="4e00b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e00b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e00b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e00b-109">Permission type</span></span>                        | <span data-ttu-id="4e00b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e00b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4e00b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e00b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e00b-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e00b-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="4e00b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e00b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e00b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e00b-114">Not supported.</span></span>                              |
| <span data-ttu-id="4e00b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e00b-115">Application</span></span>                            | <span data-ttu-id="4e00b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e00b-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="4e00b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e00b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="4e00b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e00b-118">Request headers</span></span>

| <span data-ttu-id="4e00b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4e00b-119">Name</span></span>          | <span data-ttu-id="4e00b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e00b-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4e00b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e00b-121">Authorization</span></span> | <span data-ttu-id="4e00b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e00b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e00b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e00b-124">Content-type</span></span> | <span data-ttu-id="4e00b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e00b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e00b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e00b-127">Request body</span></span>

<span data-ttu-id="4e00b-128">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e00b-128">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>
<span data-ttu-id="4e00b-129">Необходимо установить свойство контейнера **plannerPlan.**</span><span class="sxs-lookup"><span data-stu-id="4e00b-129">The **plannerPlan** container property must be set.</span></span>

><span data-ttu-id="4e00b-130">**Примечание:** Если контейнер — это группа Microsoft 365, пользователь, создавший план, должен быть членом группы, которая будет содержать план.</span><span class="sxs-lookup"><span data-stu-id="4e00b-130">**Note:** If the container is a Microsoft 365 group, the user who is creating the plan must be a member of the group that will contain the plan.</span></span> <span data-ttu-id="4e00b-131">При создании группы с помощью средства [создания группы](../api/group-post-groups.md) вы не становитесь ее участником.</span><span class="sxs-lookup"><span data-stu-id="4e00b-131">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="4e00b-132">После создания группы добавьте себя в качестве участника с помощью операции [добавления участников группы](../api/group-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="4e00b-132">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="4e00b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e00b-133">Response</span></span>

<span data-ttu-id="4e00b-134">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4e00b-134">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="4e00b-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4e00b-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4e00b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4e00b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e00b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e00b-139">Request</span></span>

<span data-ttu-id="4e00b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e00b-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e00b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e00b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 140

{
  "container": {
    "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
  },
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4e00b-142">C#</span><span class="sxs-lookup"><span data-stu-id="4e00b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e00b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e00b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e00b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e00b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e00b-145">Java</span><span class="sxs-lookup"><span data-stu-id="4e00b-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerplan-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4e00b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e00b-146">Response</span></span>

<span data-ttu-id="4e00b-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e00b-147">Here is an example of the response.</span></span> 

><span data-ttu-id="4e00b-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4e00b-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 544

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "b108ebf3-4e22-b93d-5234-dae5874656d7"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874",
    "containerId": "ebf3b108-5234-4e22-b93d-656d7dae5874",
    "type": "group"
  },
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


