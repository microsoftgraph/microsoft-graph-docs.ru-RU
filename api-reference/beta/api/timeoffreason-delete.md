---
title: Удаление Тимеоффреасон
description: ПоМетка Тимеоффреасон как неактивной с помощью задания свойства GetProperty
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: adf5c7b25f2a0fada834f5d865958cba89673df3
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657681"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="40917-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="40917-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40917-104">ПоМечайте Тимеоффреасон как неактивную \*\*\*\* , устанавливая свойство [](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="40917-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="40917-105">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="40917-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="40917-106">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="40917-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="40917-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40917-107">Permissions</span></span>

<span data-ttu-id="40917-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40917-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40917-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40917-110">Permission type</span></span>      | <span data-ttu-id="40917-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40917-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40917-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40917-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40917-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40917-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40917-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40917-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40917-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40917-115">Not supported.</span></span>    |
|<span data-ttu-id="40917-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40917-116">Application</span></span> | <span data-ttu-id="40917-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40917-117">Not supported.</span></span> |

> <span data-ttu-id="40917-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="40917-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="40917-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="40917-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="40917-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40917-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="40917-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40917-121">Request headers</span></span>

| <span data-ttu-id="40917-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40917-122">Header</span></span>       | <span data-ttu-id="40917-123">Значение</span><span class="sxs-lookup"><span data-stu-id="40917-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40917-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40917-124">Authorization</span></span>  | <span data-ttu-id="40917-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40917-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40917-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40917-127">Content-Type</span></span>  | <span data-ttu-id="40917-128">application/json</span><span class="sxs-lookup"><span data-stu-id="40917-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40917-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40917-129">Request body</span></span>
<span data-ttu-id="40917-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40917-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40917-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="40917-131">Response</span></span>

<span data-ttu-id="40917-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40917-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40917-134">Пример</span><span class="sxs-lookup"><span data-stu-id="40917-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="40917-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="40917-135">Request</span></span>

<span data-ttu-id="40917-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40917-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="40917-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="40917-137">Response</span></span>

<span data-ttu-id="40917-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40917-138">The following is an example of the response.</span></span> 

><span data-ttu-id="40917-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40917-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
