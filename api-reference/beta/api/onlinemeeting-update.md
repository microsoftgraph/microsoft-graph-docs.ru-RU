---
title: Обновление Онлинемитинг
description: Обновление свойств собрания по сети.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 56a316e69f247842d38c5e5f606d986d0600cbc9
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224738"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="03a4b-103">Обновление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="03a4b-103">Update onlineMeeting</span></span>

<span data-ttu-id="03a4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03a4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a4b-105">Обновление свойств **startDateTime**, **endDateTime**, **участников**и **субъекта** указанного [онлинемитинг](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="03a4b-105">Update the **startDateTime**, **endDateTime**, **participants**, and **subject** properties of the specified [onlineMeeting](../resources/onlinemeeting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03a4b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03a4b-106">Permissions</span></span>

| <span data-ttu-id="03a4b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03a4b-107">Permission type</span></span> | <span data-ttu-id="03a4b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03a4b-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="03a4b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03a4b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="03a4b-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03a4b-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="03a4b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03a4b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03a4b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03a4b-112">Not Supported.</span></span>                         |
| <span data-ttu-id="03a4b-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="03a4b-113">Application</span></span>                            | <span data-ttu-id="03a4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03a4b-114">Not Supported.</span></span>                                  |


## <a name="http-request"></a><span data-ttu-id="03a4b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03a4b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03a4b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03a4b-116">Request headers</span></span>
| <span data-ttu-id="03a4b-117">Имя</span><span class="sxs-lookup"><span data-stu-id="03a4b-117">Name</span></span>          | <span data-ttu-id="03a4b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="03a4b-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="03a4b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03a4b-119">Authorization</span></span> | <span data-ttu-id="03a4b-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03a4b-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03a4b-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03a4b-122">Content-type</span></span>  | <span data-ttu-id="03a4b-p102">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03a4b-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03a4b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03a4b-125">Request body</span></span>
<span data-ttu-id="03a4b-126">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03a4b-126">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="03a4b-127">Можно изменить только свойства **startDateTime**, **endDateTime**, **Участники**и **subject** .</span><span class="sxs-lookup"><span data-stu-id="03a4b-127">Only the **startDateTime**, **endDateTime**, **participants**, and **subject** properties can be modified.</span></span> <span data-ttu-id="03a4b-128">**StartDateTime** и **endDateTime** должны указываться парами.</span><span class="sxs-lookup"><span data-stu-id="03a4b-128">The **startDateTime** and **endDateTime** must appear in pairs.</span></span>

## <a name="response"></a><span data-ttu-id="03a4b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03a4b-129">Response</span></span>
<span data-ttu-id="03a4b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03a4b-130">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03a4b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="03a4b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03a4b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03a4b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="03a4b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="03a4b-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03a4b-134">C#</span><span class="sxs-lookup"><span data-stu-id="03a4b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-onlinemeeting-request-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03a4b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03a4b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-onlinemeeting-request-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03a4b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03a4b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-onlinemeeting-request-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03a4b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="03a4b-137">Response</span></span>

><span data-ttu-id="03a4b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="03a4b-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
