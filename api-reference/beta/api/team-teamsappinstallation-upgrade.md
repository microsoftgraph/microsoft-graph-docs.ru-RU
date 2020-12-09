---
title: 'Теамсаппинсталлатион: обновление'
description: Обновление установки приложения в команде
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05b275469e44c2915b60df4c08ac04048147ef3d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607744"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="b52da-103">Теамсаппинсталлатион: обновление</span><span class="sxs-lookup"><span data-stu-id="b52da-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="b52da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52da-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="b52da-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="b52da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b52da-106">Permissions</span></span>

<span data-ttu-id="b52da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b52da-109">Permission type</span></span>      | <span data-ttu-id="b52da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b52da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b52da-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b52da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b52da-112">Теамсаппинсталлатион. Реадвритефортеам, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b52da-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b52da-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b52da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b52da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52da-114">Not supported.</span></span>    |
|<span data-ttu-id="b52da-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b52da-115">Application</span></span> | <span data-ttu-id="b52da-116">Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b52da-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b52da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b52da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="b52da-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b52da-118">Request headers</span></span>

| <span data-ttu-id="b52da-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b52da-119">Header</span></span>       | <span data-ttu-id="b52da-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b52da-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b52da-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b52da-121">Authorization</span></span>  | <span data-ttu-id="b52da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b52da-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b52da-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b52da-124">Request body</span></span>

<span data-ttu-id="b52da-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b52da-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b52da-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52da-126">Response</span></span>

<span data-ttu-id="b52da-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b52da-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52da-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b52da-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b52da-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b52da-130">Request</span></span>

<span data-ttu-id="b52da-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b52da-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp_in_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade
```


### <a name="response"></a><span data-ttu-id="b52da-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52da-132">Response</span></span>

<span data-ttu-id="b52da-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b52da-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp_in_team",
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
  "description": "Upgrade app in team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


