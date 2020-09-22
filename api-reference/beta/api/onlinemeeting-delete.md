---
title: Удаление Онлинемитинг
description: Удаление собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b25330207d5785b5cb76d4d956fdff48afbf4753
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058762"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="52d62-103">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="52d62-103">Delete onlineMeeting</span></span>

<span data-ttu-id="52d62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52d62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52d62-105">Удаление объекта [онлинемитинг](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="52d62-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52d62-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52d62-106">Permissions</span></span>

| <span data-ttu-id="52d62-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52d62-107">Permission type</span></span>                        | <span data-ttu-id="52d62-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52d62-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="52d62-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52d62-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="52d62-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52d62-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="52d62-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52d62-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52d62-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52d62-112">Not Supported.</span></span>                              |
| <span data-ttu-id="52d62-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52d62-113">Application</span></span>                            | <span data-ttu-id="52d62-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="52d62-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="52d62-115">\* Администраторы должны создать [политику доступа к приложениям](/graph/cloud-communication-online-meeting-application-access-policy) и предоставить ее пользователю, достигая имени приложения, настроенного в политике, чтобы удалить собрание по сети от имени этого пользователя (идентификатор пользователя, указанный в пути реукест).</span><span class="sxs-lookup"><span data-stu-id="52d62-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to delete an online meeting on behalf of that user (user ID specified in the reuqest path) has created.</span></span>

## <a name="http-request"></a><span data-ttu-id="52d62-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52d62-116">HTTP request</span></span>

<span data-ttu-id="52d62-117">Запрос при использовании делегированного маркера</span><span class="sxs-lookup"><span data-stu-id="52d62-117">Request when using a delegated token</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

<span data-ttu-id="52d62-118">Запрос при использовании маркера приложения:</span><span class="sxs-lookup"><span data-stu-id="52d62-118">Request when using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="52d62-119">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="52d62-119">**Note:**</span></span>
>
> - <span data-ttu-id="52d62-120">`userId` — Это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="52d62-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="52d62-121">Дополнительные сведения см. в разделе [Политика доступа к приложениям](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="52d62-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="52d62-122">`meetingId` — **идентификатор** [объекта онлинемитинг](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="52d62-122">`meetingId` is the **id** of an [onlineMeeting entity](../resources/onlinemeeting.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52d62-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52d62-123">Request headers</span></span>
| <span data-ttu-id="52d62-124">Имя</span><span class="sxs-lookup"><span data-stu-id="52d62-124">Name</span></span>          | <span data-ttu-id="52d62-125">Описание</span><span class="sxs-lookup"><span data-stu-id="52d62-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="52d62-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52d62-126">Authorization</span></span> | <span data-ttu-id="52d62-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52d62-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52d62-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52d62-129">Request body</span></span>
<span data-ttu-id="52d62-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52d62-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52d62-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="52d62-131">Response</span></span>
<span data-ttu-id="52d62-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="52d62-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52d62-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="52d62-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52d62-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="52d62-135">Request</span></span>
<span data-ttu-id="52d62-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52d62-136">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="52d62-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="52d62-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="52d62-138">C#</span><span class="sxs-lookup"><span data-stu-id="52d62-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52d62-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52d62-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52d62-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52d62-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52d62-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="52d62-141">Response</span></span>

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


