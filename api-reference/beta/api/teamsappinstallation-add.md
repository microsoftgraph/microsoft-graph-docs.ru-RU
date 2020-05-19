---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05b3189825d4cfba12c000113a653595f9f7c9a3
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290492"
---
# <a name="add-app-to-team"></a><span data-ttu-id="623db-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="623db-103">Add app to team</span></span>

<span data-ttu-id="623db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="623db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="623db-105">Устанавливает [приложение](../resources/teamsapp.md) в указанную [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="623db-105">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="623db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="623db-106">Permissions</span></span>

<span data-ttu-id="623db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="623db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="623db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="623db-109">Permission type</span></span>      | <span data-ttu-id="623db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="623db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="623db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="623db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="623db-112">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623db-112">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="623db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="623db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="623db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="623db-114">Not supported.</span></span>    |
|<span data-ttu-id="623db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="623db-115">Application</span></span> | <span data-ttu-id="623db-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623db-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="623db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="623db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="623db-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="623db-118">Request headers</span></span>

| <span data-ttu-id="623db-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="623db-119">Header</span></span>       | <span data-ttu-id="623db-120">Значение</span><span class="sxs-lookup"><span data-stu-id="623db-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="623db-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="623db-121">Authorization</span></span>  | <span data-ttu-id="623db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="623db-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="623db-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="623db-124">Request body</span></span>

| <span data-ttu-id="623db-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="623db-125">Property</span></span>   | <span data-ttu-id="623db-126">Тип</span><span class="sxs-lookup"><span data-stu-id="623db-126">Type</span></span> |<span data-ttu-id="623db-127">Описание</span><span class="sxs-lookup"><span data-stu-id="623db-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="623db-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="623db-128">teamsApp</span></span>|<span data-ttu-id="623db-129">String</span><span class="sxs-lookup"><span data-stu-id="623db-129">String</span></span>|<span data-ttu-id="623db-130">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="623db-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="623db-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="623db-131">Response</span></span>

<span data-ttu-id="623db-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="623db-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="623db-134">Пример</span><span class="sxs-lookup"><span data-stu-id="623db-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="623db-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="623db-135">Request</span></span>

<span data-ttu-id="623db-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="623db-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="623db-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="623db-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_teamsApp"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="623db-138">C#</span><span class="sxs-lookup"><span data-stu-id="623db-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="623db-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="623db-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="623db-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="623db-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="623db-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="623db-141">Response</span></span>

<span data-ttu-id="623db-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="623db-142">The following is an example of the response.</span></span>

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
