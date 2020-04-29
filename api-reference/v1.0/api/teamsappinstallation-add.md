---
title: Добавление приложения в команду
description: Установка приложения для указанной команды.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 85b0a94c3892bd31ff89d286697a7193a62cd771
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509309"
---
# <a name="add-app-to-team"></a><span data-ttu-id="08992-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="08992-103">Add app to team</span></span>

<span data-ttu-id="08992-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08992-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08992-105">Установка [приложения](../resources/teamsapp.md) для указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="08992-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08992-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08992-106">Permissions</span></span>

<span data-ttu-id="08992-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08992-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08992-109">Permission type</span></span>      | <span data-ttu-id="08992-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08992-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08992-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08992-111">Delegated (work or school account)</span></span> | <span data-ttu-id="08992-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08992-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="08992-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08992-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08992-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08992-114">Not supported.</span></span>    |
|<span data-ttu-id="08992-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08992-115">Application</span></span> | <span data-ttu-id="08992-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08992-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08992-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08992-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="08992-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08992-118">Request headers</span></span>

| <span data-ttu-id="08992-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08992-119">Header</span></span>       | <span data-ttu-id="08992-120">Значение</span><span class="sxs-lookup"><span data-stu-id="08992-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08992-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08992-121">Authorization</span></span>  | <span data-ttu-id="08992-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08992-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08992-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08992-124">Request body</span></span>

| <span data-ttu-id="08992-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="08992-125">Property</span></span>   | <span data-ttu-id="08992-126">Тип</span><span class="sxs-lookup"><span data-stu-id="08992-126">Type</span></span> |<span data-ttu-id="08992-127">Описание</span><span class="sxs-lookup"><span data-stu-id="08992-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08992-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="08992-128">teamsApp</span></span>| [<span data-ttu-id="08992-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="08992-129">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="08992-130">Добавляемое приложение.</span><span class="sxs-lookup"><span data-stu-id="08992-130">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="08992-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="08992-131">Response</span></span>

<span data-ttu-id="08992-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08992-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08992-134">Пример</span><span class="sxs-lookup"><span data-stu-id="08992-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="08992-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="08992-135">Request</span></span>

<span data-ttu-id="08992-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08992-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08992-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="08992-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="08992-138">C#</span><span class="sxs-lookup"><span data-stu-id="08992-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08992-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08992-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08992-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08992-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08992-141">Java</span><span class="sxs-lookup"><span data-stu-id="08992-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08992-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="08992-142">Response</span></span>

<span data-ttu-id="08992-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08992-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
