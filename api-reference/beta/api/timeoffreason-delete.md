---
title: Удаление Тимеоффреасон
description: ПоМетка Тимеоффреасон как неактивной с помощью задания свойства GetProperty
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 74cf9ac748facb8693db1a6260cd3fbb08014068
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335117"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="f7e94-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="f7e94-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7e94-104">ПоМечайте Тимеоффреасон как неактивную \*\*\*\* , устанавливая свойство [](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="f7e94-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="f7e94-105">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="f7e94-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="f7e94-106">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="f7e94-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e94-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e94-107">Permissions</span></span>

<span data-ttu-id="f7e94-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e94-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e94-110">Permission type</span></span>      | <span data-ttu-id="f7e94-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e94-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7e94-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e94-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7e94-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e94-115">Not supported.</span></span>    |
|<span data-ttu-id="f7e94-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7e94-116">Application</span></span> | <span data-ttu-id="f7e94-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e94-117">Not supported.</span></span> |

> <span data-ttu-id="f7e94-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f7e94-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f7e94-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f7e94-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f7e94-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e94-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="f7e94-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e94-121">Request headers</span></span>

| <span data-ttu-id="f7e94-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7e94-122">Header</span></span>       | <span data-ttu-id="f7e94-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f7e94-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7e94-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7e94-124">Authorization</span></span>  | <span data-ttu-id="f7e94-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e94-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7e94-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7e94-127">Content-Type</span></span>  | <span data-ttu-id="f7e94-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f7e94-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7e94-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7e94-129">Request body</span></span>
<span data-ttu-id="f7e94-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7e94-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e94-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7e94-131">Response</span></span>

<span data-ttu-id="f7e94-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e94-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e94-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f7e94-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f7e94-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e94-135">Request</span></span>

<span data-ttu-id="f7e94-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7e94-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="f7e94-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e94-137">Response</span></span>

<span data-ttu-id="f7e94-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e94-138">The following is an example of the response.</span></span> 

><span data-ttu-id="f7e94-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7e94-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
