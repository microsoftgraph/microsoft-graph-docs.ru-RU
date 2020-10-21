---
title: Обновление Онлинемитинг
description: Обновление свойств собрания по сети.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f8a221a030e4672146b1187d4bcfdbd3f0513ceb
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635600"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="bab7b-103">Обновление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="bab7b-103">Update onlineMeeting</span></span>

<span data-ttu-id="bab7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab7b-105">Обновление свойств **startDateTime**, **endDateTime**, **участников**и **субъекта** указанного [онлинемитинг](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="bab7b-105">Update the **startDateTime**, **endDateTime**, **participants**, and **subject** properties of the specified [onlineMeeting](../resources/onlinemeeting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bab7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bab7b-106">Permissions</span></span>

| <span data-ttu-id="bab7b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bab7b-107">Permission type</span></span>                        | <span data-ttu-id="bab7b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bab7b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bab7b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bab7b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="bab7b-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bab7b-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="bab7b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bab7b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab7b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bab7b-112">Not Supported.</span></span>                              |
| <span data-ttu-id="bab7b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bab7b-113">Application</span></span>                            | <span data-ttu-id="bab7b-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="bab7b-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="bab7b-115">\* Администраторы должны создать [политику доступа к приложениям](/graph/cloud-communication-online-meeting-application-access-policy) и предоставить ее пользователю, доставке приложения, настроенного в политике, для обновления собраний по сети от имени этого пользователя (идентификатора пользователя, указанного в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="bab7b-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="bab7b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bab7b-116">HTTP request</span></span>

<span data-ttu-id="bab7b-117">Запрос с помощью делегированного маркера:</span><span class="sxs-lookup"><span data-stu-id="bab7b-117">Request using a delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

<span data-ttu-id="bab7b-118">Запрос с помощью маркера приложения:</span><span class="sxs-lookup"><span data-stu-id="bab7b-118">Request using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="bab7b-119">**Примечания:**</span><span class="sxs-lookup"><span data-stu-id="bab7b-119">**Notes:**</span></span>
>
> - <span data-ttu-id="bab7b-120">`userId` — Это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="bab7b-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="bab7b-121">Дополнительные сведения см. в разделе [Политика доступа к приложениям](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="bab7b-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="bab7b-122">`meetingId` — **идентификатор** [объекта онлинемитинг](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="bab7b-122">`meetingId` is the **id** of an [onlineMeeting entity](../resources/onlinemeeting.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab7b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bab7b-123">Request headers</span></span>
| <span data-ttu-id="bab7b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="bab7b-124">Name</span></span>          | <span data-ttu-id="bab7b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bab7b-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="bab7b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bab7b-126">Authorization</span></span> | <span data-ttu-id="bab7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bab7b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bab7b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bab7b-129">Content-type</span></span>  | <span data-ttu-id="bab7b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bab7b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bab7b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bab7b-132">Request body</span></span>
<span data-ttu-id="bab7b-133">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bab7b-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="bab7b-134">Можно изменить только свойства **startDateTime**, **endDateTime**, **Участники**и **subject** .</span><span class="sxs-lookup"><span data-stu-id="bab7b-134">Only the **startDateTime**, **endDateTime**, **participants**, and **subject** properties can be modified.</span></span> <span data-ttu-id="bab7b-135">**StartDateTime** и **endDateTime** должны указываться парами.</span><span class="sxs-lookup"><span data-stu-id="bab7b-135">The **startDateTime** and **endDateTime** must appear in pairs.</span></span>

## <a name="response"></a><span data-ttu-id="bab7b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bab7b-136">Response</span></span>
<span data-ttu-id="bab7b-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bab7b-137">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bab7b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="bab7b-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bab7b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bab7b-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bab7b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bab7b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_onlinemeeting_request"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="bab7b-141">C#</span><span class="sxs-lookup"><span data-stu-id="bab7b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-onlinemeeting-request-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bab7b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bab7b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-onlinemeeting-request-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bab7b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bab7b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-onlinemeeting-request-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bab7b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bab7b-144">Response</span></span>

><span data-ttu-id="bab7b-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bab7b-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"{id}",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"number",
      "tollFreeNumber":null,
      "dialinUrl":"url"
   }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


