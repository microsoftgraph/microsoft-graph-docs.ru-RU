---
title: Установка приложения для пользователя
description: Установка приложения в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 984157470aeceb019e234aa11c3bd693bcc6b9b0
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564090"
---
# <a name="install-app-for-user"></a><span data-ttu-id="2b261-103">Установка приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="2b261-103">Install app for user</span></span>

<span data-ttu-id="2b261-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b261-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b261-105">Установка [приложения](../resources/teamsapp.md) в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2b261-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b261-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b261-106">Permissions</span></span>

<span data-ttu-id="2b261-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b261-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b261-109">Permission type</span></span>      | <span data-ttu-id="2b261-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b261-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b261-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b261-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b261-112">Теамсаппинсталлатион. Реадвритеселффорусер, Теамсаппинсталлатион. Реадвритефорусер, TeamsAppInstallation. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b261-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="2b261-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b261-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b261-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b261-114">Not supported.</span></span>    |
|<span data-ttu-id="2b261-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b261-115">Application</span></span> | <span data-ttu-id="2b261-116">Теамсаппинсталлатион. Реадвритеселффорусер. ALL, Теамсаппинсталлатион. Реадвритефорусер. ALL, TeamsAppInstallation. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b261-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b261-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b261-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="2b261-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b261-118">Request headers</span></span>

| <span data-ttu-id="2b261-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b261-119">Header</span></span>       | <span data-ttu-id="2b261-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2b261-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b261-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b261-121">Authorization</span></span>  | <span data-ttu-id="2b261-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b261-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b261-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b261-124">Content-type</span></span> | <span data-ttu-id="2b261-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b261-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b261-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b261-127">Request body</span></span>

<span data-ttu-id="2b261-128">В тексте запроса должен содержаться идентификатор существующего приложения каталога, который требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="2b261-128">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="2b261-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b261-129">Property</span></span>   | <span data-ttu-id="2b261-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2b261-130">Type</span></span> |<span data-ttu-id="2b261-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2b261-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b261-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2b261-132">teamsApp</span></span>|<span data-ttu-id="2b261-133">String</span><span class="sxs-lookup"><span data-stu-id="2b261-133">String</span></span>|<span data-ttu-id="2b261-134">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="2b261-134">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="2b261-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b261-135">Response</span></span>

<span data-ttu-id="2b261-p104">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b261-p104">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b261-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2b261-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b261-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b261-139">Request</span></span>

<span data-ttu-id="2b261-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b261-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->

```http
POST https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="2b261-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b261-141">Response</span></span>
<span data-ttu-id="2b261-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b261-142">The following is an example of the response.</span></span>

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
