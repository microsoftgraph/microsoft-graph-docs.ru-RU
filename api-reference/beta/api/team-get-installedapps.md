---
title: Получение установленного приложения в команде
description: Получение приложения, установленного в команде.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 49903514fb6345978d90ca1df7a8ab5279c61410
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564204"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="b3589-103">Получение установленного приложения в команде</span><span class="sxs-lookup"><span data-stu-id="b3589-103">Get installed app in team</span></span>

<span data-ttu-id="b3589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3589-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3589-105">Получение [приложения](../resources/teamsappinstallation.md) , установленного в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b3589-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3589-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3589-106">Permissions</span></span>

<span data-ttu-id="b3589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3589-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3589-109">Permission type</span></span>      | <span data-ttu-id="b3589-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3589-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3589-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3589-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3589-112">Теамсаппинсталлатион. Реадвритеселффортеам, Теамсаппинсталлатион. Реадфорусер, Теамсаппинсталлатион. ReadForTeam, TeamsAppInstallation. ReadWriteForTeam, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3589-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b3589-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3589-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3589-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3589-114">Not supported.</span></span>    |
|<span data-ttu-id="b3589-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3589-115">Application</span></span> | <span data-ttu-id="b3589-116">Теамсаппинсталлатион. Реадвритеселффортеам, Теамсаппинсталлатион. Реадфортеам. ALL, Теамсаппинсталлатион. ReadWriteForTeam. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3589-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3589-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3589-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3589-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3589-118">Request headers</span></span>

| <span data-ttu-id="b3589-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3589-119">Header</span></span>       | <span data-ttu-id="b3589-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b3589-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3589-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3589-121">Authorization</span></span>  | <span data-ttu-id="b3589-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3589-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3589-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3589-124">Request body</span></span>

<span data-ttu-id="b3589-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3589-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3589-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3589-126">Response</span></span>

<span data-ttu-id="b3589-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3589-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3589-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3589-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="b3589-129">Пример 1: получение установленного приложения</span><span class="sxs-lookup"><span data-stu-id="b3589-129">Example 1: Get the installed app</span></span>
#### <a name="request"></a><span data-ttu-id="b3589-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3589-130">Request</span></span>

<span data-ttu-id="b3589-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3589-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```

---

#### <a name="response"></a><span data-ttu-id="b3589-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3589-132">Response</span></span>

<span data-ttu-id="b3589-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3589-133">The following is an example of the response.</span></span>
><span data-ttu-id="b3589-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3589-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
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

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="b3589-136">Пример 2: получение имен и других сведений об установленном приложении</span><span class="sxs-lookup"><span data-stu-id="b3589-136">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="b3589-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3589-137">Request</span></span>

<span data-ttu-id="b3589-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3589-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```

---

#### <a name="response"></a><span data-ttu-id="b3589-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3589-139">Response</span></span>

<span data-ttu-id="b3589-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3589-140">The following is an example of the response.</span></span>

><span data-ttu-id="b3589-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3589-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
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
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "beta"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

