---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f40951eb3c33b638542a8e2210911adffb15a444
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908329"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="ab5a9-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="ab5a9-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab5a9-104">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab5a9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5a9-105">Permissions</span></span>

<span data-ttu-id="ab5a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab5a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab5a9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab5a9-108">Permission type</span></span>      | <span data-ttu-id="ab5a9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab5a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab5a9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab5a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab5a9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab5a9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab5a9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab5a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab5a9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-113">Not supported.</span></span>    |
|<span data-ttu-id="ab5a9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab5a9-114">Application</span></span> | <span data-ttu-id="ab5a9-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab5a9-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab5a9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab5a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="ab5a9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab5a9-117">Request headers</span></span>

| <span data-ttu-id="ab5a9-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab5a9-118">Header</span></span>       | <span data-ttu-id="ab5a9-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ab5a9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab5a9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab5a9-120">Authorization</span></span>  | <span data-ttu-id="ab5a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab5a9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab5a9-123">Request body</span></span>

<span data-ttu-id="ab5a9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab5a9-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab5a9-125">Response</span></span>

<span data-ttu-id="ab5a9-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab5a9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ab5a9-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab5a9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab5a9-129">Request</span></span>

<span data-ttu-id="ab5a9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="ab5a9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab5a9-131">Response</span></span>

<span data-ttu-id="ab5a9-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ab5a9-132">The following is an example of the response.</span></span> 

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
