---
title: Удаление Тимеофф
description: Удаление экземпляра Тимеофф по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe3fdbe8445b11c9d1c0f176bccdc794e3a80480
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657492"
---
# <a name="delete-timeoff"></a><span data-ttu-id="baa0d-103">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="baa0d-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baa0d-104">Удаление экземпляра [тимеофф](../resources/timeoff.md) по расписанию [](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="baa0d-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="baa0d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="baa0d-105">Permissions</span></span>

<span data-ttu-id="baa0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baa0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baa0d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baa0d-108">Permission type</span></span>      | <span data-ttu-id="baa0d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="baa0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baa0d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baa0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="baa0d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa0d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="baa0d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baa0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baa0d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baa0d-113">Not supported.</span></span>    |
|<span data-ttu-id="baa0d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baa0d-114">Application</span></span> | <span data-ttu-id="baa0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baa0d-115">Not supported.</span></span> |

> <span data-ttu-id="baa0d-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="baa0d-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="baa0d-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="baa0d-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="baa0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baa0d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="baa0d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="baa0d-119">Request headers</span></span>

| <span data-ttu-id="baa0d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="baa0d-120">Header</span></span>       | <span data-ttu-id="baa0d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="baa0d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="baa0d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="baa0d-122">Authorization</span></span>  | <span data-ttu-id="baa0d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baa0d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="baa0d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="baa0d-125">Content-Type</span></span>  | <span data-ttu-id="baa0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="baa0d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="baa0d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="baa0d-127">Request body</span></span>
<span data-ttu-id="baa0d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="baa0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baa0d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="baa0d-129">Response</span></span>

<span data-ttu-id="baa0d-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="baa0d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baa0d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="baa0d-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="baa0d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="baa0d-133">Request</span></span>

<span data-ttu-id="baa0d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baa0d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="baa0d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="baa0d-135">Response</span></span>

<span data-ttu-id="baa0d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="baa0d-136">The following is an example of the response.</span></span> 

><span data-ttu-id="baa0d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baa0d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
