---
title: 'Опеншифтчанжерекуест: утверждение'
description: Утверждение запроса Опеншифтчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 148b4c52a6f288d961c949cc0d599cb468c8b322
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155070"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="0fde6-103">Опеншифтчанжерекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="0fde6-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="0fde6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fde6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fde6-105">Утверждение объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="0fde6-105">Approve an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fde6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fde6-106">Permissions</span></span>

<span data-ttu-id="0fde6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fde6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fde6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fde6-109">Permission type</span></span>                        | <span data-ttu-id="0fde6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fde6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0fde6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fde6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fde6-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0fde6-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0fde6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fde6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fde6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fde6-114">Not supported.</span></span> |
| <span data-ttu-id="0fde6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fde6-115">Application</span></span>                            | <span data-ttu-id="0fde6-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fde6-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="0fde6-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="0fde6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0fde6-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="0fde6-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0fde6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fde6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="0fde6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fde6-120">Request headers</span></span>

| <span data-ttu-id="0fde6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0fde6-121">Name</span></span>          | <span data-ttu-id="0fde6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0fde6-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0fde6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fde6-123">Authorization</span></span> | <span data-ttu-id="0fde6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fde6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0fde6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fde6-126">Content-type</span></span> | <span data-ttu-id="0fde6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fde6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fde6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fde6-129">Request body</span></span>

<span data-ttu-id="0fde6-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0fde6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0fde6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="0fde6-131">Parameter</span></span>    | <span data-ttu-id="0fde6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0fde6-132">Type</span></span>        | <span data-ttu-id="0fde6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0fde6-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0fde6-134">message</span><span class="sxs-lookup"><span data-stu-id="0fde6-134">message</span></span>|<span data-ttu-id="0fde6-135">String</span><span class="sxs-lookup"><span data-stu-id="0fde6-135">String</span></span>|<span data-ttu-id="0fde6-136">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="0fde6-136">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="0fde6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fde6-137">Response</span></span>

<span data-ttu-id="0fde6-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0fde6-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fde6-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="0fde6-140">Examples</span></span>

<span data-ttu-id="0fde6-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0fde6-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0fde6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fde6-142">Request</span></span>

<span data-ttu-id="0fde6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fde6-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="0fde6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fde6-144">Response</span></span>

<span data-ttu-id="0fde6-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0fde6-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
