---
title: Получить установленное приложение для пользователя
description: Получение приложения, установленного в личной области указанного пользователя.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 393a0663136ec167645a93cfcedd776758ed88d2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564219"
---
# <a name="get-installed-app-for-user"></a><span data-ttu-id="1ee48-103">Получить установленное приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="1ee48-103">Get installed app for user</span></span>

<span data-ttu-id="1ee48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ee48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ee48-105">Получение [приложения](../resources/teamsappinstallation.md) , установленного в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="1ee48-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ee48-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ee48-106">Permissions</span></span>

<span data-ttu-id="1ee48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ee48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ee48-109">Permission type</span></span>      | <span data-ttu-id="1ee48-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ee48-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ee48-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ee48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee48-112">Теамсаппинсталлатион. Реадфорусер, Теамсаппинсталлатион. Read, Теамсаппинсталлатион. Реадвритеселффорусер, TeamsAppInstallation. ReadWriteForUser, TeamsAppInstallation. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee48-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.Read, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="1ee48-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ee48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ee48-114">Not supported.</span></span>    |
|<span data-ttu-id="1ee48-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1ee48-115">Application</span></span> | <span data-ttu-id="1ee48-116">Теамсаппинсталлатион. Реадфорусер. ALL, Теамсаппинсталлатион. Read. ALL, Теамсаппинсталлатион. Реадвритеселффорусер. ALL, TeamsAppInstallation. ReadWriteForUser. ALL, TeamsAppInstallation. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1ee48-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.Read.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ee48-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1ee48-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ee48-118">Request headers</span></span>

| <span data-ttu-id="1ee48-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ee48-119">Header</span></span>       | <span data-ttu-id="1ee48-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1ee48-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ee48-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ee48-121">Authorization</span></span>  | <span data-ttu-id="1ee48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ee48-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ee48-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ee48-124">Request body</span></span>

<span data-ttu-id="1ee48-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ee48-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ee48-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ee48-126">Response</span></span>

<span data-ttu-id="1ee48-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и [приложение](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ee48-127">If successful, this method returns a `200 OK` response code and an [app](../resources/teamsappinstallation.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ee48-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ee48-128">Examples</span></span>

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a><span data-ttu-id="1ee48-129">Пример 1: получение приложения, установленного для указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="1ee48-129">Example 1: Get an app installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="1ee48-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ee48-130">Request</span></span>

<span data-ttu-id="1ee48-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ee48-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```

#### <a name="response"></a><span data-ttu-id="1ee48-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ee48-132">Response</span></span>

<span data-ttu-id="1ee48-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ee48-133">The following is an example of the response.</span></span>
><span data-ttu-id="1ee48-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ee48-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
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
      "id": "id-value"
    }
  ]
}
```
### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a><span data-ttu-id="1ee48-136">Пример 2: получение имен и других сведений о приложении, установленном для пользователя</span><span class="sxs-lookup"><span data-stu-id="1ee48-136">Example 2: Get the names and other details of the app installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="1ee48-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ee48-137">Request</span></span>

<span data-ttu-id="1ee48-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ee48-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
}-->
```http
GET https://graph.microsoft.com/beta/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="1ee48-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ee48-139">Response</span></span>

<span data-ttu-id="1ee48-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ee48-140">The following is an example of the response.</span></span>

><span data-ttu-id="1ee48-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ee48-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
          "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('5b649834-7412-4cce-9e69-176e95a394f5')/installedApps(teamsAppDefinition())/$entity",
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
