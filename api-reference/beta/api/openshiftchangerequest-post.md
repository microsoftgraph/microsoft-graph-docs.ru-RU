---
title: Создание Опеншифтчанжерекуест
description: Создайте экземпляр объекта Опеншифтчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 04957803bd8c907bfad8fafb17d9c548e856e16c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071908"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="52155-103">Создание Опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="52155-103">Create openShiftChangeRequest</span></span>

<span data-ttu-id="52155-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52155-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52155-105">Создание экземпляра объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="52155-105">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="52155-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52155-106">Permissions</span></span>

<span data-ttu-id="52155-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52155-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52155-109">Permission type</span></span>                        | <span data-ttu-id="52155-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52155-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52155-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52155-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52155-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52155-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="52155-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52155-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52155-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52155-114">Not supported.</span></span> |
| <span data-ttu-id="52155-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52155-115">Application</span></span>                            | <span data-ttu-id="52155-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="52155-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="52155-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="52155-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="52155-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52155-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52155-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52155-119">Optional query parameters</span></span>

<span data-ttu-id="52155-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="52155-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="52155-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="52155-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52155-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52155-122">Request headers</span></span>

| <span data-ttu-id="52155-123">Имя</span><span class="sxs-lookup"><span data-stu-id="52155-123">Name</span></span>      |<span data-ttu-id="52155-124">Описание</span><span class="sxs-lookup"><span data-stu-id="52155-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52155-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52155-125">Authorization</span></span> | <span data-ttu-id="52155-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52155-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52155-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52155-128">Content-type</span></span> | <span data-ttu-id="52155-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52155-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52155-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52155-131">Request body</span></span>
<span data-ttu-id="52155-132">В тексте запроса укажите представление объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52155-132">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="52155-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="52155-133">Response</span></span>

<span data-ttu-id="52155-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и созданный объект [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52155-134">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52155-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="52155-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52155-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="52155-136">Request</span></span>

<span data-ttu-id="52155-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52155-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="52155-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="52155-138">Response</span></span>

<span data-ttu-id="52155-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="52155-139">The following is an example of the response.</span></span>

> <span data-ttu-id="52155-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52155-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


