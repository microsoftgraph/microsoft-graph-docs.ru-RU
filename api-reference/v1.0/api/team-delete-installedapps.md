---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 159f355514cab6f1ffb230f26c95208e58e416b6
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607437"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="7f5e3-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="7f5e3-103">Remove app from team</span></span>

<span data-ttu-id="7f5e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f5e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f5e3-105">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7f5e3-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f5e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f5e3-106">Permissions</span></span>

<span data-ttu-id="7f5e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f5e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f5e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f5e3-109">Permission type</span></span>      | <span data-ttu-id="7f5e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f5e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f5e3-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f5e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f5e3-112">Теамсаппинсталлатион. Реадвритефортеам, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7f5e3-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="7f5e3-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f5e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f5e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f5e3-114">Not supported.</span></span>    |
|<span data-ttu-id="7f5e3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f5e3-115">Application</span></span> | <span data-ttu-id="7f5e3-116">Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7f5e3-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f5e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f5e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="7f5e3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f5e3-118">Request headers</span></span>

| <span data-ttu-id="7f5e3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f5e3-119">Header</span></span>       | <span data-ttu-id="7f5e3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7f5e3-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f5e3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f5e3-121">Authorization</span></span>  | <span data-ttu-id="7f5e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f5e3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f5e3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f5e3-124">Request body</span></span>

<span data-ttu-id="7f5e3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f5e3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f5e3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f5e3-126">Response</span></span>

<span data-ttu-id="7f5e3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7f5e3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f5e3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7f5e3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f5e3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f5e3-130">Request</span></span>

<span data-ttu-id="7f5e3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f5e3-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp_in_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```

### <a name="response"></a><span data-ttu-id="7f5e3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f5e3-132">Response</span></span>

<span data-ttu-id="7f5e3-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7f5e3-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp_in_team",
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
  "description": "Remove app from team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


