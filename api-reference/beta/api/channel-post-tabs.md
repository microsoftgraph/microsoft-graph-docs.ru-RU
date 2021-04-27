---
title: Добавление вкладки в канал
description: 'Добавляет (закрепляет) вкладку в указанный канал в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5575c4ae9267a968c7381ba4a89b66f9e0e7698d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047541"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="8c440-103">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="8c440-103">Add tab to channel</span></span>

<span data-ttu-id="8c440-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c440-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c440-105">Добавляет (закрепляет) [вкладку](../resources/teamstab.md) в указанный [канал](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8c440-105">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="8c440-106">Соответствующее приложение уже должно быть [установлено в команде](../api/team-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="8c440-106">The corresponding app must already be [installed in the team](../api/team-list-installedapps.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c440-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c440-107">Permissions</span></span>
<span data-ttu-id="8c440-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c440-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c440-110">Permission type</span></span>      | <span data-ttu-id="8c440-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c440-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c440-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c440-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c440-113">TeamsTab.Create, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c440-113">TeamsTab.Create, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8c440-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c440-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c440-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c440-115">Not supported.</span></span>    |
| <span data-ttu-id="8c440-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c440-116">Application</span></span>   | <span data-ttu-id="8c440-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c440-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="8c440-118">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8c440-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="8c440-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8c440-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8c440-120">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="8c440-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8c440-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c440-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="8c440-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c440-122">Request headers</span></span>
| <span data-ttu-id="8c440-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c440-123">Header</span></span>       | <span data-ttu-id="8c440-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8c440-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c440-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c440-125">Authorization</span></span>  | <span data-ttu-id="8c440-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c440-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c440-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c440-128">Request body</span></span>

<span data-ttu-id="8c440-129">[teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="8c440-129">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="8c440-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c440-130">Response</span></span>

<span data-ttu-id="8c440-131">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="8c440-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c440-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8c440-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8c440-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c440-133">Request</span></span>

<span data-ttu-id="8c440-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c440-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="8c440-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c440-135">Response</span></span>

<span data-ttu-id="8c440-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c440-136">The following is an example of the response.</span></span> <span data-ttu-id="8c440-137">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c440-137">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="8c440-138">См. также</span><span class="sxs-lookup"><span data-stu-id="8c440-138">See also</span></span>

- [<span data-ttu-id="8c440-139">Настройка типов вкладок buit-in</span><span class="sxs-lookup"><span data-stu-id="8c440-139">Configuring the buit-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="8c440-140">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="8c440-140">Add app to team</span></span>](team-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


