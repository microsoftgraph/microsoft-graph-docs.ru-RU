---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c717ca93c832736671f856a6454bcf0de877681c
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908465"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="f121c-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="f121c-103">Upgrade an app in a team</span></span>

<span data-ttu-id="f121c-104">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="f121c-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="f121c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f121c-105">Permissions</span></span>

<span data-ttu-id="f121c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f121c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f121c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f121c-108">Permission type</span></span>      | <span data-ttu-id="f121c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f121c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f121c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f121c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f121c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f121c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f121c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f121c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f121c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f121c-113">Not supported.</span></span>    |
|<span data-ttu-id="f121c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f121c-114">Application</span></span> | <span data-ttu-id="f121c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f121c-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="f121c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f121c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="f121c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f121c-117">Request headers</span></span>

| <span data-ttu-id="f121c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f121c-118">Header</span></span>       | <span data-ttu-id="f121c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f121c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f121c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f121c-120">Authorization</span></span>  | <span data-ttu-id="f121c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f121c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f121c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f121c-123">Request body</span></span>

<span data-ttu-id="f121c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f121c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f121c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f121c-125">Response</span></span>

<span data-ttu-id="f121c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f121c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f121c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f121c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f121c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f121c-129">Request</span></span>

<span data-ttu-id="f121c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f121c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="f121c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f121c-131">Response</span></span>

<span data-ttu-id="f121c-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f121c-132">The following is an example of the response.</span></span> 

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
