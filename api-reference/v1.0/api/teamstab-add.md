---
title: Добавление вкладки в канал
description: 'Добавляет (закрепляет) вкладку в указанный канал в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 53246826dc7b15b240a9b8a0c72d3177bd7aa06d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978337"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="bb9bc-103">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="bb9bc-103">Add tab to channel</span></span>

<span data-ttu-id="bb9bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb9bc-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="bb9bc-105">Добавляет (закрепляет) [вкладку](../resources/teamstab.md) в указанный [канал](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bb9bc-105">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="bb9bc-106">Соответствующее приложение уже должно быть [установлено в команде](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="bb9bc-106">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb9bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9bc-107">Permissions</span></span>
<span data-ttu-id="bb9bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb9bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9bc-110">Permission type</span></span>      | <span data-ttu-id="bb9bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb9bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb9bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb9bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb9bc-113">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9bc-113">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bb9bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb9bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb9bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-115">Not supported.</span></span>    |
| <span data-ttu-id="bb9bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb9bc-116">Application</span></span>                            |<span data-ttu-id="bb9bc-117">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9bc-117">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bb9bc-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bb9bc-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bb9bc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb9bc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="bb9bc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb9bc-121">Request headers</span></span>
| <span data-ttu-id="bb9bc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb9bc-122">Header</span></span>       | <span data-ttu-id="bb9bc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bb9bc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb9bc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb9bc-124">Authorization</span></span>  | <span data-ttu-id="bb9bc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb9bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb9bc-127">Request body</span></span>

<span data-ttu-id="bb9bc-128">[teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="bb9bc-128">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="bb9bc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb9bc-129">Response</span></span>

<span data-ttu-id="bb9bc-130">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-130">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb9bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb9bc-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb9bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb9bc-132">Request</span></span>

<span data-ttu-id="bb9bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="bb9bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb9bc-134">Response</span></span>

<span data-ttu-id="bb9bc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-135">The following is an example of the response.</span></span> <span data-ttu-id="bb9bc-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bb9bc-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb9bc-137">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bb9bc-138">См. также</span><span class="sxs-lookup"><span data-stu-id="bb9bc-138">See also</span></span>

[<span data-ttu-id="bb9bc-139">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="bb9bc-139">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

