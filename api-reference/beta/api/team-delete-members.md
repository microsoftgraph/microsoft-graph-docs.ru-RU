---
title: Удаление участников из группы
description: Удаление Конверсатионмембер из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ad51fddf0acf4499271ffeb3c02e0433e52dedb
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051150"
---
# <a name="delete-members"></a><span data-ttu-id="8be1c-103">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="8be1c-103">Delete members</span></span>
<span data-ttu-id="8be1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8be1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8be1c-105">Удаление нового [конверсатионмембер](../resources/conversationmember.md) из [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8be1c-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8be1c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8be1c-106">Permissions</span></span>
<span data-ttu-id="8be1c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8be1c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8be1c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8be1c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8be1c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8be1c-109">Permission type</span></span>|<span data-ttu-id="8be1c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8be1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8be1c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8be1c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8be1c-112">Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8be1c-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="8be1c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8be1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8be1c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8be1c-114">Not supported.</span></span>    |
|<span data-ttu-id="8be1c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8be1c-115">Application</span></span>| <span data-ttu-id="8be1c-116">Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8be1c-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8be1c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8be1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="8be1c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8be1c-118">Request headers</span></span>
|<span data-ttu-id="8be1c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8be1c-119">Name</span></span>|<span data-ttu-id="8be1c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8be1c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8be1c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8be1c-121">Authorization</span></span>|<span data-ttu-id="8be1c-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8be1c-122">Bearer {token}.</span></span> <span data-ttu-id="8be1c-123">Required.</span><span class="sxs-lookup"><span data-stu-id="8be1c-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8be1c-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8be1c-124">Request body</span></span>
<span data-ttu-id="8be1c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8be1c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8be1c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8be1c-126">Response</span></span>

<span data-ttu-id="8be1c-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8be1c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8be1c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8be1c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8be1c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8be1c-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### <a name="response"></a><span data-ttu-id="8be1c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8be1c-130">Response</span></span>
<span data-ttu-id="8be1c-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8be1c-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

