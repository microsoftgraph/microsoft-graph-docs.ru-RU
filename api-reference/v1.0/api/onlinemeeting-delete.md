---
title: Удаление onlineMeeting
description: Удаление собрания в Интернете.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8af5125d227c09ec2d115aabf626fc3b737d4085
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896566"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="8fb4c-103">Удаление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8fb4c-103">Delete onlineMeeting</span></span>

<span data-ttu-id="8fb4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fb4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fb4c-105">Удаление [объекта onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="8fb4c-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fb4c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fb4c-106">Permissions</span></span>

| <span data-ttu-id="8fb4c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fb4c-107">Permission type</span></span> | <span data-ttu-id="8fb4c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fb4c-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="8fb4c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fb4c-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="8fb4c-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fb4c-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="8fb4c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fb4c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fb4c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb4c-112">Not Supported.</span></span>                         |
| <span data-ttu-id="8fb4c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fb4c-113">Application</span></span>                            | <span data-ttu-id="8fb4c-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="8fb4c-114">OnlineMeetings.ReadWrite.All\*</span></span>          |

> [!IMPORTANT]
> <span data-ttu-id="8fb4c-115">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенного в политике, удалить онлайн-собрание от имени этого пользователя (пользовательский ID, указанный в пути reuqest).</span><span class="sxs-lookup"><span data-stu-id="8fb4c-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to delete an online meeting on behalf of that user (user ID specified in the reuqest path) has created.</span></span>

## <a name="http-request"></a><span data-ttu-id="8fb4c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fb4c-116">HTTP request</span></span>
<span data-ttu-id="8fb4c-117">Удаление указанного onlineMeeting путем собрания ID с делегированным разрешением:</span><span class="sxs-lookup"><span data-stu-id="8fb4c-117">To delete the specified onlineMeeting by meeting ID with delegated permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="8fb4c-118">Удаление указанного onlineMeeting путем встречи с ИД с разрешением приложения:</span><span class="sxs-lookup"><span data-stu-id="8fb4c-118">To delete the specified onlineMeeting by meeting ID with application permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{userId}/onlineMeetings/{meetingId}
```
> [!NOTE]
> - <span data-ttu-id="8fb4c-119">`userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="8fb4c-119">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="8fb4c-120">Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="8fb4c-120">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="8fb4c-121">`meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="8fb4c-121">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fb4c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fb4c-122">Request headers</span></span>
| <span data-ttu-id="8fb4c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8fb4c-123">Name</span></span>          | <span data-ttu-id="8fb4c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8fb4c-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8fb4c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fb4c-125">Authorization</span></span> | <span data-ttu-id="8fb4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fb4c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fb4c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8fb4c-128">Request body</span></span>
<span data-ttu-id="8fb4c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fb4c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fb4c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fb4c-130">Response</span></span>
<span data-ttu-id="8fb4c-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8fb4c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8fb4c-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="8fb4c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8fb4c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fb4c-134">Request</span></span>
<span data-ttu-id="8fb4c-135">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fb4c-135">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8fb4c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fb4c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype"],
  "name": "delete-call-2"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="8fb4c-137">C#</span><span class="sxs-lookup"><span data-stu-id="8fb4c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fb4c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fb4c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fb4c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fb4c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8fb4c-140">Java</span><span class="sxs-lookup"><span data-stu-id="8fb4c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8fb4c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fb4c-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

