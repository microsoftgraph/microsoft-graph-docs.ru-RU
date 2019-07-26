---
title: Установка приложения для пользователя
description: Установка приложения в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 009d2efe115d8b07f9bdead07965d402db65e65a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908546"
---
# <a name="install-app-for-user"></a><span data-ttu-id="b70b7-103">Установка приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="b70b7-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b70b7-104">Установка [приложения](../resources/teamsapp.md) в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b70b7-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b70b7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b70b7-105">Permissions</span></span>

<span data-ttu-id="b70b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b70b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b70b7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b70b7-108">Permission type</span></span>      | <span data-ttu-id="b70b7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b70b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b70b7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b70b7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b70b7-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b70b7-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="b70b7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b70b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b70b7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b70b7-113">Not supported.</span></span>    |
|<span data-ttu-id="b70b7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b70b7-114">Application</span></span> | <span data-ttu-id="b70b7-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b70b7-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b70b7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b70b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="b70b7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b70b7-117">Request headers</span></span>

| <span data-ttu-id="b70b7-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b70b7-118">Header</span></span>       | <span data-ttu-id="b70b7-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b70b7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b70b7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b70b7-120">Authorization</span></span>  | <span data-ttu-id="b70b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b70b7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b70b7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b70b7-123">Request body</span></span>

<span data-ttu-id="b70b7-124">В тексте запроса должен содержаться идентификатор существующего приложения каталога, который требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="b70b7-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="b70b7-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="b70b7-125">Property</span></span>   | <span data-ttu-id="b70b7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b70b7-126">Type</span></span> |<span data-ttu-id="b70b7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b70b7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b70b7-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b70b7-128">teamsApp</span></span>|<span data-ttu-id="b70b7-129">String</span><span class="sxs-lookup"><span data-stu-id="b70b7-129">String</span></span>|<span data-ttu-id="b70b7-130">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="b70b7-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="b70b7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b70b7-131">Response</span></span>

<span data-ttu-id="b70b7-p103">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b70b7-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b70b7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b70b7-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b70b7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b70b7-135">Request</span></span>

<span data-ttu-id="b70b7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b70b7-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="b70b7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b70b7-137">Response</span></span>

<span data-ttu-id="b70b7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b70b7-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
