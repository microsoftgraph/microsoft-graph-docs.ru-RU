---
title: Получить установленное приложение для пользователя
description: Извлечение приложения, установленного в личном поле указанного пользователя.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0c714decf64b140c4f440ac671e2db50c0893a29
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696179"
---
# <a name="get-installed-app-for-user"></a><span data-ttu-id="a18e1-103">Получить установленное приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="a18e1-103">Get installed app for user</span></span>

<span data-ttu-id="a18e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a18e1-105">[Извлечение приложения,](../resources/teamsappinstallation.md) установленного в личном поле указанного [пользователя.](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="a18e1-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a18e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a18e1-106">Permissions</span></span>

<span data-ttu-id="a18e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a18e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a18e1-109">Permission type</span></span>      | <span data-ttu-id="a18e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a18e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a18e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a18e1-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="a18e1-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="a18e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a18e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18e1-114">Not supported.</span></span>    |
|<span data-ttu-id="a18e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a18e1-115">Application</span></span> | <span data-ttu-id="a18e1-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="a18e1-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a18e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a18e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id | user-principal-name}/teamwork/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="a18e1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a18e1-118">Request headers</span></span>

| <span data-ttu-id="a18e1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a18e1-119">Header</span></span>       | <span data-ttu-id="a18e1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a18e1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a18e1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a18e1-121">Authorization</span></span>  | <span data-ttu-id="a18e1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a18e1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a18e1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a18e1-124">Request body</span></span>

<span data-ttu-id="a18e1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a18e1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a18e1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18e1-126">Response</span></span>

<span data-ttu-id="a18e1-127">В случае успешной работы этот метод возвращает код `200 OK` ответа и приложение [в](../resources/teamsappinstallation.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a18e1-127">If successful, this method returns a `200 OK` response code and an [app](../resources/teamsappinstallation.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a18e1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a18e1-128">Examples</span></span>

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a><span data-ttu-id="a18e1-129">Пример 1. Установить приложение для указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="a18e1-129">Example 1: Get an app installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="a18e1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a18e1-130">Request</span></span>

<span data-ttu-id="a18e1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a18e1-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a18e1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a18e1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```
# <a name="c"></a>[<span data-ttu-id="a18e1-133">C#</span><span class="sxs-lookup"><span data-stu-id="a18e1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a18e1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a18e1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a18e1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a18e1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a18e1-136">Java</span><span class="sxs-lookup"><span data-stu-id="a18e1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a18e1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18e1-137">Response</span></span>

<span data-ttu-id="a18e1-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a18e1-138">The following is an example of the response.</span></span>
><span data-ttu-id="a18e1-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a18e1-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a><span data-ttu-id="a18e1-140">Пример 2. Получить имена и другие сведения о приложении, установленном для пользователя</span><span class="sxs-lookup"><span data-stu-id="a18e1-140">Example 2: Get the names and other details of the app installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="a18e1-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a18e1-141">Request</span></span>

<span data-ttu-id="a18e1-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a18e1-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="a18e1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18e1-143">Response</span></span>

<span data-ttu-id="a18e1-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a18e1-144">The following is an example of the response.</span></span>

><span data-ttu-id="a18e1-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a18e1-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('5b649834-7412-4cce-9e69-176e95a394f5')/installedApps(teamsAppDefinition())/$entity",
      "id": "NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=",
      "teamsAppDefinition": {
        "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk=",
        "teamsAppId": "a6b63365-31a4-4f43-92ec-710b71557af9",
        "displayName": "Power Apps",
        "version": "0.9"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User get teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
