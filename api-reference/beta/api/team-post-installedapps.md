---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную команду.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 93610704438fef36cabaa4d14e33e05a69a183bc
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690435"
---
# <a name="add-app-to-team"></a><span data-ttu-id="608b2-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="608b2-103">Add app to team</span></span>

<span data-ttu-id="608b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="608b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="608b2-105">Установите приложение [для](../resources/teamsapp.md) указанной [команды.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="608b2-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="608b2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="608b2-106">Permissions</span></span>

<span data-ttu-id="608b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="608b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="608b2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="608b2-109">Permission type</span></span>      | <span data-ttu-id="608b2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="608b2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="608b2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="608b2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="608b2-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="608b2-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="608b2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="608b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="608b2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="608b2-114">Not supported.</span></span>    |
|<span data-ttu-id="608b2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="608b2-115">Application</span></span> | <span data-ttu-id="608b2-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="608b2-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="608b2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="608b2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="608b2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="608b2-118">Request headers</span></span>

| <span data-ttu-id="608b2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="608b2-119">Header</span></span>       | <span data-ttu-id="608b2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="608b2-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="608b2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="608b2-121">Authorization</span></span>  | <span data-ttu-id="608b2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="608b2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="608b2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="608b2-124">Request body</span></span>

| <span data-ttu-id="608b2-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="608b2-125">Property</span></span>   | <span data-ttu-id="608b2-126">Тип</span><span class="sxs-lookup"><span data-stu-id="608b2-126">Type</span></span> |<span data-ttu-id="608b2-127">Описание</span><span class="sxs-lookup"><span data-stu-id="608b2-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="608b2-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="608b2-128">teamsApp</span></span>|<span data-ttu-id="608b2-129">String</span><span class="sxs-lookup"><span data-stu-id="608b2-129">String</span></span>|<span data-ttu-id="608b2-130">ИД добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="608b2-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="608b2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="608b2-131">Response</span></span>

<span data-ttu-id="608b2-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="608b2-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="608b2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="608b2-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="608b2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="608b2-135">Request</span></span>

<span data-ttu-id="608b2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="608b2-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="608b2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="608b2-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="608b2-138">C#</span><span class="sxs-lookup"><span data-stu-id="608b2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-app-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="608b2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="608b2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-app-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="608b2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="608b2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-app-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="608b2-141">Java</span><span class="sxs-lookup"><span data-stu-id="608b2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-app-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="608b2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="608b2-142">Response</span></span>

<span data-ttu-id="608b2-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="608b2-143">The following is an example of the response.</span></span>

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


