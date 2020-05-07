---
title: Создание Опеншифтчанжерекуест
description: Создайте экземпляр объекта Опеншифтчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f8f6469b92a8d2fbc289cfa436f2ed97c2204c00
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155049"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="83a45-103">Создание Опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="83a45-103">Create openShiftChangeRequest</span></span>

<span data-ttu-id="83a45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83a45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83a45-105">Создание экземпляра объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="83a45-105">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83a45-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83a45-106">Permissions</span></span>

<span data-ttu-id="83a45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83a45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83a45-109">Permission type</span></span>                        | <span data-ttu-id="83a45-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83a45-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83a45-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83a45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83a45-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="83a45-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="83a45-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83a45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83a45-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83a45-114">Not supported.</span></span> |
| <span data-ttu-id="83a45-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83a45-115">Application</span></span>                            | <span data-ttu-id="83a45-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83a45-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="83a45-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="83a45-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="83a45-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="83a45-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="83a45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83a45-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="83a45-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83a45-120">Request headers</span></span>

| <span data-ttu-id="83a45-121">Имя</span><span class="sxs-lookup"><span data-stu-id="83a45-121">Name</span></span>      |<span data-ttu-id="83a45-122">Описание</span><span class="sxs-lookup"><span data-stu-id="83a45-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83a45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83a45-123">Authorization</span></span> | <span data-ttu-id="83a45-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83a45-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83a45-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83a45-126">Content-type</span></span> | <span data-ttu-id="83a45-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83a45-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83a45-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83a45-129">Request body</span></span>
<span data-ttu-id="83a45-130">В тексте запроса укажите представление объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83a45-130">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83a45-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="83a45-131">Response</span></span>

<span data-ttu-id="83a45-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и созданный объект [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83a45-132">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83a45-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="83a45-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83a45-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="83a45-134">Request</span></span>

<span data-ttu-id="83a45-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83a45-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="83a45-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="83a45-136">Response</span></span>

<span data-ttu-id="83a45-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83a45-137">The following is an example of the response.</span></span>

> <span data-ttu-id="83a45-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83a45-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "assignedTo": "manager",
  "state": "pending",
  "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
  "senderDateTime": "2019-05-01T10:00:00Z",
  "senderMessage": "Can I take this shift?",
  "managerUserId": null,
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create openShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
