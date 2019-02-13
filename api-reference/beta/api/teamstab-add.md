---
title: Добавление вкладки в канал
description: 'Добавляет (закрепляет) вкладку в указанный канал в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5235cc7dd99098fce1bdad437a74d65e6a437742
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967230"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="205fb-103">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="205fb-103">Add tab to channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="205fb-104">Добавляет (закрепляет) [вкладку](../resources/teamstab.md) в указанный [канал](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="205fb-104">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="205fb-105">Соответствующее приложение уже должно быть [установлено в команде](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="205fb-105">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="205fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="205fb-106">Permissions</span></span>
<span data-ttu-id="205fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="205fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="205fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="205fb-109">Permission type</span></span>      | <span data-ttu-id="205fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="205fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="205fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="205fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="205fb-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="205fb-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="205fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="205fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="205fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="205fb-114">Not supported.</span></span>    |
| <span data-ttu-id="205fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="205fb-115">Application</span></span>                            | <span data-ttu-id="205fb-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="205fb-116">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="205fb-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="205fb-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="205fb-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="205fb-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="205fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="205fb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="205fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="205fb-120">Request headers</span></span>
| <span data-ttu-id="205fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="205fb-121">Header</span></span>       | <span data-ttu-id="205fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="205fb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="205fb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="205fb-123">Authorization</span></span>  | <span data-ttu-id="205fb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="205fb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="205fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="205fb-126">Request body</span></span>

<span data-ttu-id="205fb-127">[teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="205fb-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="205fb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="205fb-128">Response</span></span>

<span data-ttu-id="205fb-129">В случае успешного выполнения этот метод возвращает код отклика `201 OK`.</span><span class="sxs-lookup"><span data-stu-id="205fb-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="205fb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="205fb-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="205fb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="205fb-131">Request</span></span>

<span data-ttu-id="205fb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="205fb-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="205fb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="205fb-133">Response</span></span>

<span data-ttu-id="205fb-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="205fb-134">The following is an example of the response.</span></span> <span data-ttu-id="205fb-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="205fb-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="205fb-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="205fb-136">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="205fb-137">См. также</span><span class="sxs-lookup"><span data-stu-id="205fb-137">See also</span></span>

[<span data-ttu-id="205fb-138">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="205fb-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
