---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8fde83a82e1c46b8b37cfedea2a202b8d339ea2d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607680"
---
# <a name="add-app-to-team"></a><span data-ttu-id="fbedb-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="fbedb-103">Add app to team</span></span>

<span data-ttu-id="fbedb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbedb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbedb-105">Установка [приложения](../resources/teamsapp.md) для указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fbedb-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbedb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbedb-106">Permissions</span></span>

<span data-ttu-id="fbedb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbedb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbedb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbedb-109">Permission type</span></span>      | <span data-ttu-id="fbedb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbedb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbedb-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbedb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fbedb-112">Теамсаппинсталлатион. Реадвритефортеам, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fbedb-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="fbedb-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbedb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbedb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbedb-114">Not supported.</span></span>    |
|<span data-ttu-id="fbedb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fbedb-115">Application</span></span> | <span data-ttu-id="fbedb-116">Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fbedb-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbedb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbedb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="fbedb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbedb-118">Request headers</span></span>

| <span data-ttu-id="fbedb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbedb-119">Header</span></span>       | <span data-ttu-id="fbedb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fbedb-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbedb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbedb-121">Authorization</span></span>  | <span data-ttu-id="fbedb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbedb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbedb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbedb-124">Request body</span></span>

| <span data-ttu-id="fbedb-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbedb-125">Property</span></span>   | <span data-ttu-id="fbedb-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fbedb-126">Type</span></span> |<span data-ttu-id="fbedb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fbedb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbedb-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="fbedb-128">teamsApp</span></span>|<span data-ttu-id="fbedb-129">String</span><span class="sxs-lookup"><span data-stu-id="fbedb-129">String</span></span>|<span data-ttu-id="fbedb-130">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="fbedb-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="fbedb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbedb-131">Response</span></span>

<span data-ttu-id="fbedb-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fbedb-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbedb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fbedb-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbedb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbedb-135">Request</span></span>

<span data-ttu-id="fbedb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbedb-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_app_in_team"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="fbedb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbedb-137">Response</span></span>

<span data-ttu-id="fbedb-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fbedb-138">The following is an example of the response.</span></span>

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


