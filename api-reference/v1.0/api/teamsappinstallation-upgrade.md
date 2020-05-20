---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 132da552f6ed587e80b21474c4c2ca3a69935ca6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290434"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="18816-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="18816-103">Upgrade an app in a team</span></span>

<span data-ttu-id="18816-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18816-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18816-105">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="18816-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="18816-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18816-106">Permissions</span></span>

<span data-ttu-id="18816-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18816-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18816-109">Permission type</span></span>      | <span data-ttu-id="18816-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18816-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18816-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18816-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18816-112">TeamsApp. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="18816-112">TeamsApp.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="18816-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18816-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18816-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18816-114">Not supported.</span></span>    |
|<span data-ttu-id="18816-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18816-115">Application</span></span> | <span data-ttu-id="18816-116">TeamsApp. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="18816-116">TeamsApp.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18816-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18816-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="18816-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18816-118">Request headers</span></span>

| <span data-ttu-id="18816-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18816-119">Header</span></span>       | <span data-ttu-id="18816-120">Значение</span><span class="sxs-lookup"><span data-stu-id="18816-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18816-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18816-121">Authorization</span></span>  | <span data-ttu-id="18816-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18816-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18816-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18816-124">Request body</span></span>

<span data-ttu-id="18816-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18816-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18816-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="18816-126">Response</span></span>

<span data-ttu-id="18816-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="18816-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18816-129">Пример</span><span class="sxs-lookup"><span data-stu-id="18816-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="18816-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="18816-130">Request</span></span>

<span data-ttu-id="18816-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18816-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18816-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="18816-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="18816-133">C#</span><span class="sxs-lookup"><span data-stu-id="18816-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18816-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18816-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18816-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18816-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18816-136">Java</span><span class="sxs-lookup"><span data-stu-id="18816-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18816-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="18816-137">Response</span></span>

<span data-ttu-id="18816-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18816-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
