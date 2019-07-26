---
title: Добавление приложения в команду
description: Установка приложения для указанной команды.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 07e8a5989050a0323fdbcde8027e6c89bef0d454
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908468"
---
# <a name="add-app-to-team"></a><span data-ttu-id="b491f-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="b491f-103">Add app to team</span></span>

<span data-ttu-id="b491f-104">Установка [приложения](../resources/teamsapp.md) для указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b491f-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b491f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b491f-105">Permissions</span></span>

<span data-ttu-id="b491f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b491f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b491f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b491f-108">Permission type</span></span>      | <span data-ttu-id="b491f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b491f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b491f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b491f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b491f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b491f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b491f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b491f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b491f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b491f-113">Not supported.</span></span>    |
|<span data-ttu-id="b491f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b491f-114">Application</span></span> | <span data-ttu-id="b491f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b491f-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b491f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b491f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="b491f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b491f-117">Request headers</span></span>

| <span data-ttu-id="b491f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b491f-118">Header</span></span>       | <span data-ttu-id="b491f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b491f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b491f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b491f-120">Authorization</span></span>  | <span data-ttu-id="b491f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b491f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b491f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b491f-123">Request body</span></span>

| <span data-ttu-id="b491f-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="b491f-124">Property</span></span>   | <span data-ttu-id="b491f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b491f-125">Type</span></span> |<span data-ttu-id="b491f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b491f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b491f-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b491f-127">teamsApp</span></span>| [<span data-ttu-id="b491f-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b491f-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="b491f-129">Добавляемое приложение.</span><span class="sxs-lookup"><span data-stu-id="b491f-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="b491f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b491f-130">Response</span></span>

<span data-ttu-id="b491f-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b491f-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b491f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b491f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b491f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b491f-134">Request</span></span>

<span data-ttu-id="b491f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b491f-135">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="b491f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b491f-136">Response</span></span>

<span data-ttu-id="b491f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b491f-137">The following is an example of the response.</span></span>

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
