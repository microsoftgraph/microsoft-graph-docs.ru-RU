---
title: Удаление объекта schedulingGroup
description: Пометка элемента Счедулингграуп как неактивного путем задания его свойства "свойство Active"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 793b6ed249d5eb3dfde6b3667c4bfaafe89a9fde
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972075"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="db2bf-103">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="db2bf-103">Delete schedulingGroup</span></span>

<span data-ttu-id="db2bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db2bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db2bf-105">Помечайте [счедулингграуп](../resources/schedulinggroup.md) как неактивную, устанавливая **его свойство** GetProperty.</span><span class="sxs-lookup"><span data-stu-id="db2bf-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="db2bf-106">Этот метод не удаляет [счедулингграуп](../resources/schedulinggroup.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="db2bf-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="db2bf-107">Существующие [сменные](../resources/shift.md) экземпляры, назначенные группе планирования, не входят в группу.</span><span class="sxs-lookup"><span data-stu-id="db2bf-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="db2bf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db2bf-108">Permissions</span></span>

<span data-ttu-id="db2bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db2bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db2bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db2bf-111">Permission type</span></span>      | <span data-ttu-id="db2bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db2bf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db2bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db2bf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db2bf-114">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="db2bf-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="db2bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db2bf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db2bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2bf-116">Not supported.</span></span>    |
|<span data-ttu-id="db2bf-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="db2bf-117">Application</span></span> | <span data-ttu-id="db2bf-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db2bf-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db2bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db2bf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="db2bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db2bf-120">Request headers</span></span>

| <span data-ttu-id="db2bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db2bf-121">Header</span></span>       | <span data-ttu-id="db2bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db2bf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db2bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db2bf-123">Authorization</span></span>  | <span data-ttu-id="db2bf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db2bf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db2bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db2bf-126">Request body</span></span>
<span data-ttu-id="db2bf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db2bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db2bf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2bf-128">Response</span></span>

<span data-ttu-id="db2bf-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db2bf-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db2bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="db2bf-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="db2bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db2bf-132">Request</span></span>

<span data-ttu-id="db2bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db2bf-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db2bf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db2bf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="db2bf-135">C#</span><span class="sxs-lookup"><span data-stu-id="db2bf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db2bf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db2bf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db2bf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db2bf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db2bf-138">Java</span><span class="sxs-lookup"><span data-stu-id="db2bf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-delete-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db2bf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2bf-139">Response</span></span>

<span data-ttu-id="db2bf-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db2bf-140">The following is an example of the response.</span></span> 

><span data-ttu-id="db2bf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db2bf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


