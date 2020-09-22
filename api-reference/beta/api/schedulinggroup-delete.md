---
title: Удаление объекта schedulingGroup
description: Пометка элемента Счедулингграуп как неактивного путем задания его свойства "свойство Active"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9c5eabe4503bf8ac3f6d98d16a0a85a6f01d5af4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071933"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="83ff9-103">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="83ff9-103">Delete schedulingGroup</span></span>

<span data-ttu-id="83ff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83ff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83ff9-105">Помечайте [счедулингграуп](../resources/schedulinggroup.md) как неактивную, устанавливая **его свойство** GetProperty.</span><span class="sxs-lookup"><span data-stu-id="83ff9-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="83ff9-106">Этот метод не удаляет [счедулингграуп](../resources/schedulinggroup.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="83ff9-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="83ff9-107">Существующие [сменные](../resources/shift.md) экземпляры, назначенные группе планирования, не входят в группу.</span><span class="sxs-lookup"><span data-stu-id="83ff9-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="83ff9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83ff9-108">Permissions</span></span>

<span data-ttu-id="83ff9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83ff9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83ff9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83ff9-111">Permission type</span></span>      | <span data-ttu-id="83ff9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83ff9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83ff9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83ff9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="83ff9-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83ff9-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83ff9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83ff9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83ff9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83ff9-116">Not supported.</span></span>    |
|<span data-ttu-id="83ff9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83ff9-117">Application</span></span> | <span data-ttu-id="83ff9-118">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="83ff9-118">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="83ff9-119">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="83ff9-119">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="83ff9-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="83ff9-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="83ff9-121">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="83ff9-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="83ff9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83ff9-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="83ff9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83ff9-123">Request headers</span></span>

| <span data-ttu-id="83ff9-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83ff9-124">Header</span></span>       | <span data-ttu-id="83ff9-125">Значение</span><span class="sxs-lookup"><span data-stu-id="83ff9-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83ff9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83ff9-126">Authorization</span></span>  | <span data-ttu-id="83ff9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83ff9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83ff9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83ff9-129">Request body</span></span>
<span data-ttu-id="83ff9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83ff9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83ff9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="83ff9-131">Response</span></span>

<span data-ttu-id="83ff9-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83ff9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83ff9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="83ff9-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83ff9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="83ff9-135">Request</span></span>

<span data-ttu-id="83ff9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83ff9-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83ff9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="83ff9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="83ff9-138">C#</span><span class="sxs-lookup"><span data-stu-id="83ff9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83ff9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83ff9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83ff9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83ff9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="83ff9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="83ff9-141">Response</span></span>

<span data-ttu-id="83ff9-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83ff9-142">The following is an example of the response.</span></span> 

><span data-ttu-id="83ff9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83ff9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


