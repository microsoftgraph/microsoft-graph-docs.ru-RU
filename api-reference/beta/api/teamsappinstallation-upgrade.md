---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 844c868ec2898edb4ed8626b198f3025c96b4e03
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289924"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="a593e-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="a593e-103">Upgrade an app in a team</span></span>

<span data-ttu-id="a593e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a593e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a593e-105">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="a593e-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="a593e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a593e-106">Permissions</span></span>

<span data-ttu-id="a593e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a593e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a593e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a593e-109">Permission type</span></span>      | <span data-ttu-id="a593e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a593e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a593e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a593e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a593e-112">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a593e-112">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a593e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a593e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a593e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a593e-114">Not supported.</span></span>    |
|<span data-ttu-id="a593e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a593e-115">Application</span></span> | <span data-ttu-id="a593e-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a593e-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a593e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a593e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="a593e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a593e-118">Request headers</span></span>

| <span data-ttu-id="a593e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a593e-119">Header</span></span>       | <span data-ttu-id="a593e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a593e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a593e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a593e-121">Authorization</span></span>  | <span data-ttu-id="a593e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a593e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a593e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a593e-124">Request body</span></span>

<span data-ttu-id="a593e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a593e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a593e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a593e-126">Response</span></span>

<span data-ttu-id="a593e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a593e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a593e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a593e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a593e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a593e-130">Request</span></span>

<span data-ttu-id="a593e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a593e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a593e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a593e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="a593e-133">C#</span><span class="sxs-lookup"><span data-stu-id="a593e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a593e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a593e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a593e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a593e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a593e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a593e-136">Response</span></span>

<span data-ttu-id="a593e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a593e-137">The following is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
