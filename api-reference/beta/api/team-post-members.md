---
title: Добавление участника в группу
description: Добавление нового участника в группу.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9291cb0c60ed740ec9fdf1155a7f1e75e56f1705
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387838"
---
# <a name="add-member-to-team"></a><span data-ttu-id="9a34c-103">Добавление участника в группу</span><span class="sxs-lookup"><span data-stu-id="9a34c-103">Add member to team</span></span>
<span data-ttu-id="9a34c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a34c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a34c-105">Добавление нового [conversationMember](../resources/conversationmember.md) в [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9a34c-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a34c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a34c-106">Permissions</span></span>
<span data-ttu-id="9a34c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a34c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a34c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a34c-109">Permission type</span></span>|<span data-ttu-id="9a34c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a34c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a34c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a34c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="9a34c-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a34c-112">TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="9a34c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a34c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a34c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a34c-114">Not supported.</span></span>    |
|<span data-ttu-id="9a34c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9a34c-115">Application</span></span>| <span data-ttu-id="9a34c-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a34c-116">TeamMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a34c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a34c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="9a34c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a34c-118">Request headers</span></span>
|<span data-ttu-id="9a34c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9a34c-119">Name</span></span>|<span data-ttu-id="9a34c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9a34c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9a34c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a34c-121">Authorization</span></span>|<span data-ttu-id="9a34c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a34c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9a34c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a34c-124">Content-Type</span></span>|<span data-ttu-id="9a34c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a34c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a34c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a34c-127">Request body</span></span>
<span data-ttu-id="9a34c-128">В теле запроса укажите описание объекта [conversationMember](../resources/conversationmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a34c-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9a34c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a34c-129">Response</span></span>

<span data-ttu-id="9a34c-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a34c-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span> <span data-ttu-id="9a34c-131">Чтобы добиться наилучших результатов, регулируйте звонки с использованием 2-секундной буферизации.</span><span class="sxs-lookup"><span data-stu-id="9a34c-131">For best results, stagger calls with 2 seconds of buffer.</span></span>

<span data-ttu-id="9a34c-132">Чтобы добиться наилучших результатов, регулируйте звонки с использованием 2-секундной буферизации.</span><span class="sxs-lookup"><span data-stu-id="9a34c-132">For best results, stagger calls with a 2 second buffer.</span></span>

## <a name="examples"></a><span data-ttu-id="9a34c-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a34c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a34c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a34c-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9a34c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a34c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
Content-type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
}
```
# <a name="c"></a>[<span data-ttu-id="9a34c-136">C#</span><span class="sxs-lookup"><span data-stu-id="9a34c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a34c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a34c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a34c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a34c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a34c-139">Java</span><span class="sxs-lookup"><span data-stu-id="9a34c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9a34c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a34c-140">Response</span></span>
<span data-ttu-id="9a34c-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a34c-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
    "roles": [
        "owner"
    ],
    "userId": "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    "displayName": "Cameron White",
    "email": "CameronW@M365x987948.OnMicrosoft.com"
}
```

## <a name="see-also"></a><span data-ttu-id="9a34c-142">См. также</span><span class="sxs-lookup"><span data-stu-id="9a34c-142">See also</span></span>

- [<span data-ttu-id="9a34c-143">Добавление участника в канал</span><span class="sxs-lookup"><span data-stu-id="9a34c-143">Add member in channel</span></span>](channel-post-members.md)


