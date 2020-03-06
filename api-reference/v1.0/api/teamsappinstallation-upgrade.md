---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ab3a2bdce05e6cbe6b653109ef0e8faed9946e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509288"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="47c43-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="47c43-103">Upgrade an app in a team</span></span>

<span data-ttu-id="47c43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47c43-105">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="47c43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47c43-106">Permissions</span></span>

<span data-ttu-id="47c43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47c43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47c43-109">Permission type</span></span>      | <span data-ttu-id="47c43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47c43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47c43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47c43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="47c43-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c43-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47c43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47c43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47c43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c43-114">Not supported.</span></span>    |
|<span data-ttu-id="47c43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47c43-115">Application</span></span> | <span data-ttu-id="47c43-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c43-116">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="47c43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47c43-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="47c43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47c43-118">Request headers</span></span>

| <span data-ttu-id="47c43-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47c43-119">Header</span></span>       | <span data-ttu-id="47c43-120">Значение</span><span class="sxs-lookup"><span data-stu-id="47c43-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47c43-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47c43-121">Authorization</span></span>  | <span data-ttu-id="47c43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47c43-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47c43-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47c43-124">Request body</span></span>

<span data-ttu-id="47c43-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47c43-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47c43-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="47c43-126">Response</span></span>

<span data-ttu-id="47c43-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47c43-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47c43-129">Пример</span><span class="sxs-lookup"><span data-stu-id="47c43-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="47c43-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="47c43-130">Request</span></span>

<span data-ttu-id="47c43-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47c43-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47c43-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="47c43-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="47c43-133">C#</span><span class="sxs-lookup"><span data-stu-id="47c43-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47c43-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47c43-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47c43-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47c43-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47c43-136">Java</span><span class="sxs-lookup"><span data-stu-id="47c43-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47c43-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="47c43-137">Response</span></span>

<span data-ttu-id="47c43-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47c43-138">The following is an example of the response.</span></span> 

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
