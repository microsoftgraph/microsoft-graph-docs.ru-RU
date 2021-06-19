---
title: Список объектов permissionGrant команды
description: Получение объектов permissionGrant команды.
author: jecha
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 30439fab877a2de7152c7d85a81cdfb5aa818f1e
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993728"
---
# <a name="list-permissiongrants-of-a-team"></a><span data-ttu-id="d1e01-103">Список объектов permissionGrant команды</span><span class="sxs-lookup"><span data-stu-id="d1e01-103">List permissionGrants of a team</span></span>

<span data-ttu-id="d1e01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1e01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1e01-p101">Список всех [разрешений, предоставленных конкретному ресурсу](../resources/resourcespecificpermissiongrant.md) в [команде](../resources/team.md). Это список приложений Azure AD, имеющих доступ к команде, а также типов доступа, которыми обладает каждое приложение.</span><span class="sxs-lookup"><span data-stu-id="d1e01-p101">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [team](../resources/team.md). This is a list of Azure AD apps that have access to the team along with the kind of access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1e01-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e01-107">Permissions</span></span>

<span data-ttu-id="d1e01-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1e01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e01-110">Permission Type</span></span>                        | <span data-ttu-id="d1e01-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1e01-111">Permissions (from least to most privileged)</span></span>                                                                                                                                                                                                                              |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d1e01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1e01-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1e01-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadWriteForTeam</span><span class="sxs-lookup"><span data-stu-id="d1e01-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadWriteForTeam</span></span>                                                                     |
| <span data-ttu-id="d1e01-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1e01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1e01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e01-115">Not supported.</span></span>                                                                                                                                                                                                                                                           |
| <span data-ttu-id="d1e01-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d1e01-116">Application</span></span>                            | <span data-ttu-id="d1e01-117">TeamsAppInstallation.Read.Group *, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteSelfForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, TeamsApp.Read.Group*</span><span class="sxs-lookup"><span data-stu-id="d1e01-117">TeamsAppInstallation.Read.Group *, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteSelfForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, TeamsApp.Read.Group*</span></span> |

> <span data-ttu-id="d1e01-118">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d1e01-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="d1e01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1e01-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1e01-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1e01-120">Optional query parameters</span></span>

<span data-ttu-id="d1e01-121">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d1e01-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1e01-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1e01-122">Request headers</span></span>

| <span data-ttu-id="d1e01-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1e01-123">Header</span></span>           | <span data-ttu-id="d1e01-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d1e01-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="d1e01-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1e01-125">Authorization</span></span>    | <span data-ttu-id="d1e01-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1e01-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1e01-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1e01-128">Request body</span></span>

<span data-ttu-id="d1e01-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1e01-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1e01-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e01-130">Response</span></span>

<span data-ttu-id="d1e01-131">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1e01-131">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1e01-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1e01-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1e01-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1e01-133">Request</span></span>

<span data-ttu-id="d1e01-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1e01-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "team_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants
```

---

### <a name="response"></a><span data-ttu-id="d1e01-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e01-135">Response</span></span>

<span data-ttu-id="d1e01-136">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1e01-136">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#permissionGrants",
    "value": [
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNDaGF0U2V0dGluZ3MuUmVhZFdyaXRlLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        },
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamsTab.Create.Group"
        },
        {
            "id": "ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="d1e01-137">См. также</span><span class="sxs-lookup"><span data-stu-id="d1e01-137">See also</span></span>
- [<span data-ttu-id="d1e01-138">Список предоставленных разрешений группы</span><span class="sxs-lookup"><span data-stu-id="d1e01-138">List permission grants of a group</span></span>](group-list-permissionGrants.md)
- [<span data-ttu-id="d1e01-139">Список предоставленных разрешений чата</span><span class="sxs-lookup"><span data-stu-id="d1e01-139">List permission grants of a chat</span></span>](chat-list-permissionGrants.md)