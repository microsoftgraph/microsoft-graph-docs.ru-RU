---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 056543a8b1753fb9a0b4bb6e8cdfe28428ae2e01
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607351"
---
# <a name="add-app-to-team"></a><span data-ttu-id="61376-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="61376-103">Add app to team</span></span>

<span data-ttu-id="61376-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61376-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61376-105">Установка [приложения](../resources/teamsapp.md) для указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="61376-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="61376-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61376-106">Permissions</span></span>

<span data-ttu-id="61376-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61376-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61376-109">Permission type</span></span>      | <span data-ttu-id="61376-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61376-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61376-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61376-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61376-112">Теамсаппинсталлатион. Реадвритефортеам, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="61376-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="61376-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61376-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61376-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61376-114">Not supported.</span></span>    |
|<span data-ttu-id="61376-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="61376-115">Application</span></span> | <span data-ttu-id="61376-116">Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="61376-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61376-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61376-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="61376-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61376-118">Request headers</span></span>

| <span data-ttu-id="61376-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61376-119">Header</span></span>       | <span data-ttu-id="61376-120">Значение</span><span class="sxs-lookup"><span data-stu-id="61376-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61376-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61376-121">Authorization</span></span>  | <span data-ttu-id="61376-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61376-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61376-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61376-124">Request body</span></span>

| <span data-ttu-id="61376-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="61376-125">Property</span></span>   | <span data-ttu-id="61376-126">Тип</span><span class="sxs-lookup"><span data-stu-id="61376-126">Type</span></span> |<span data-ttu-id="61376-127">Описание</span><span class="sxs-lookup"><span data-stu-id="61376-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61376-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="61376-128">teamsApp</span></span>|<span data-ttu-id="61376-129">String</span><span class="sxs-lookup"><span data-stu-id="61376-129">String</span></span>|<span data-ttu-id="61376-130">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="61376-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="61376-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="61376-131">Response</span></span>

<span data-ttu-id="61376-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61376-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61376-134">Пример</span><span class="sxs-lookup"><span data-stu-id="61376-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="61376-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="61376-135">Request</span></span>

<span data-ttu-id="61376-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61376-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_app_in_team"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="61376-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="61376-137">Response</span></span>

<span data-ttu-id="61376-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="61376-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add teamsApp",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


