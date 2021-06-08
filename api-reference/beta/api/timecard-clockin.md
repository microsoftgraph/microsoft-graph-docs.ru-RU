---
title: 'timeCard: clockIn'
description: Вовремя запустите хронограф.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7075b2323bcf2792dcb58b09c248dbcc095775d2
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787942"
---
# <a name="timecard-clockin"></a><span data-ttu-id="002b1-103">timeCard: clockIn</span><span class="sxs-lookup"><span data-stu-id="002b1-103">timeCard: clockIn</span></span>

<span data-ttu-id="002b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="002b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="002b1-105">Часы, чтобы запустить [timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="002b1-105">Clock in to start a [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="002b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="002b1-106">Permissions</span></span>

<span data-ttu-id="002b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="002b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="002b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="002b1-109">Permission type</span></span>      | <span data-ttu-id="002b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="002b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="002b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="002b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="002b1-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="002b1-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="002b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="002b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="002b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="002b1-114">Not supported.</span></span>    |
|<span data-ttu-id="002b1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="002b1-115">Application</span></span> | <span data-ttu-id="002b1-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="002b1-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="002b1-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="002b1-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="002b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="002b1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/clockIn
```

## <a name="request-headers"></a><span data-ttu-id="002b1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="002b1-119">Request headers</span></span>

| <span data-ttu-id="002b1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="002b1-120">Header</span></span>       | <span data-ttu-id="002b1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="002b1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="002b1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="002b1-122">Authorization</span></span>  | <span data-ttu-id="002b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="002b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="002b1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="002b1-125">Content-type</span></span> | <span data-ttu-id="002b1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="002b1-p103">application/json. Required.</span></span>|
| <span data-ttu-id="002b1-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="002b1-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="002b1-129">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="002b1-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="002b1-130">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="002b1-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="002b1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="002b1-131">Request body</span></span>

<span data-ttu-id="002b1-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="002b1-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="002b1-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="002b1-133">Parameter</span></span>    | <span data-ttu-id="002b1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="002b1-134">Type</span></span>        | <span data-ttu-id="002b1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="002b1-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="002b1-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="002b1-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="002b1-137">Указать, происходит ли это действие в утвержденной локации.</span><span class="sxs-lookup"><span data-stu-id="002b1-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="002b1-138">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="002b1-138">onBehalfOfUserId</span></span>| <span data-ttu-id="002b1-139">String</span><span class="sxs-lookup"><span data-stu-id="002b1-139">String</span></span> | <span data-ttu-id="002b1-140">Необязательный параметр, используемый менеджером для записи от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="002b1-140">Optional parameter used by the manager to clock in on behalf of a user.</span></span>|
|<span data-ttu-id="002b1-141">notes</span><span class="sxs-lookup"><span data-stu-id="002b1-141">notes</span></span>| [<span data-ttu-id="002b1-142">itemBody</span><span class="sxs-lookup"><span data-stu-id="002b1-142">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="002b1-143">Заметки для часов.</span><span class="sxs-lookup"><span data-stu-id="002b1-143">Notes for the clock in.</span></span> |

## <a name="response"></a><span data-ttu-id="002b1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="002b1-144">Response</span></span>

<span data-ttu-id="002b1-145">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект timeCard](../resources/timeCard.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="002b1-145">If successful, this method returns a `201 Created` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="002b1-146">Пример</span><span class="sxs-lookup"><span data-stu-id="002b1-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="002b1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="002b1-147">Request</span></span>
<span data-ttu-id="002b1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="002b1-148">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="002b1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="002b1-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-clockin"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/clockin
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "clock in notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="002b1-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="002b1-150">Response</span></span>

<span data-ttu-id="002b1-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="002b1-151">The following is an example of the response.</span></span> 

><span data-ttu-id="002b1-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="002b1-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T22:58:41.327Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedIn",
    "confirmedBy": "none",
    "clockOutEvent": null,
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "breaks": [],
    "originalEntry": {
        "clockOutEvent": null,
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "breaks": []
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Clock In",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
