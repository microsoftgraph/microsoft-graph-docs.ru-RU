---
title: Удаление участников из группы
description: Удаление conversationMember из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e98aed4edc959314473d645934e8e8bfbba1143
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273692"
---
# <a name="remove-members-from-team"></a><span data-ttu-id="eec29-103">Удаление участников из группы</span><span class="sxs-lookup"><span data-stu-id="eec29-103">Remove members from team</span></span>
<span data-ttu-id="eec29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eec29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eec29-105">Удаление нового [conversationMember](../resources/conversationmember.md) из [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="eec29-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eec29-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eec29-106">Permissions</span></span>
<span data-ttu-id="eec29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eec29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eec29-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eec29-109">Permission type</span></span>|<span data-ttu-id="eec29-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eec29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eec29-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eec29-111">Delegated (work or school account)</span></span>| <span data-ttu-id="eec29-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec29-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="eec29-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eec29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eec29-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eec29-114">Not supported.</span></span>    |
|<span data-ttu-id="eec29-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="eec29-115">Application</span></span>| <span data-ttu-id="eec29-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec29-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eec29-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eec29-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="eec29-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eec29-118">Request headers</span></span>
|<span data-ttu-id="eec29-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eec29-119">Name</span></span>|<span data-ttu-id="eec29-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eec29-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eec29-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eec29-121">Authorization</span></span>|<span data-ttu-id="eec29-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eec29-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eec29-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eec29-124">Request body</span></span>
<span data-ttu-id="eec29-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eec29-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eec29-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="eec29-126">Response</span></span>

<span data-ttu-id="eec29-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eec29-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eec29-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="eec29-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eec29-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="eec29-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eec29-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="eec29-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="eec29-131">C#</span><span class="sxs-lookup"><span data-stu-id="eec29-131">C#</span></span>](#tab/csharp)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eec29-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eec29-132">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eec29-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eec29-133">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="eec29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eec29-134">Response</span></span>
<span data-ttu-id="eec29-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eec29-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
