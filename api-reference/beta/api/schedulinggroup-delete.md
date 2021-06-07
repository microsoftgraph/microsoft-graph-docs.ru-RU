---
title: Удаление объекта schedulingGroup
description: Пометить группу планирования как неактивной, установив ее свойство isActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 751d40329b06fe694c7bf0c53e9dc9499b5fee57
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788012"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="b55fa-103">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="b55fa-103">Delete schedulingGroup</span></span>

<span data-ttu-id="b55fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b55fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b55fa-105">[Пометить группу планирования](../resources/schedulinggroup.md) как неактивной, установив ее **свойство isActive.**</span><span class="sxs-lookup"><span data-stu-id="b55fa-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="b55fa-106">Этот метод не удаляет [группу планирования из](../resources/schedulinggroup.md) расписания.</span><span class="sxs-lookup"><span data-stu-id="b55fa-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="b55fa-107">[Существующие](../resources/shift.md) экземпляры переноса, назначенные группе планирования, остаются частью группы.</span><span class="sxs-lookup"><span data-stu-id="b55fa-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="b55fa-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b55fa-108">Permissions</span></span>

<span data-ttu-id="b55fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b55fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b55fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b55fa-111">Permission type</span></span>      | <span data-ttu-id="b55fa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b55fa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b55fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b55fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b55fa-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b55fa-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b55fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b55fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b55fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b55fa-116">Not supported.</span></span>    |
|<span data-ttu-id="b55fa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b55fa-117">Application</span></span> | <span data-ttu-id="b55fa-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b55fa-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b55fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b55fa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="b55fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b55fa-120">Request headers</span></span>

| <span data-ttu-id="b55fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b55fa-121">Header</span></span>       | <span data-ttu-id="b55fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b55fa-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b55fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b55fa-123">Authorization</span></span>  | <span data-ttu-id="b55fa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b55fa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b55fa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b55fa-126">Request body</span></span>
<span data-ttu-id="b55fa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b55fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b55fa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b55fa-128">Response</span></span>

<span data-ttu-id="b55fa-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b55fa-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b55fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b55fa-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b55fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b55fa-132">Request</span></span>

<span data-ttu-id="b55fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b55fa-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b55fa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b55fa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="b55fa-135">C#</span><span class="sxs-lookup"><span data-stu-id="b55fa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b55fa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b55fa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b55fa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b55fa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b55fa-138">Java</span><span class="sxs-lookup"><span data-stu-id="b55fa-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-delete-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b55fa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b55fa-139">Response</span></span>

<span data-ttu-id="b55fa-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b55fa-140">The following is an example of the response.</span></span> 

><span data-ttu-id="b55fa-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b55fa-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


