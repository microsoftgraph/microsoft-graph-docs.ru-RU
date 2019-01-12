---
title: Добавление вкладки канала
description: 'Добавляет (PIN) вкладку для указанного канала в группе. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 18b1c332939585106e1014d7f5d852e7abea431d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913403"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="fb766-103">Добавление вкладки канала</span><span class="sxs-lookup"><span data-stu-id="fb766-103">Add tab to channel</span></span>

> <span data-ttu-id="fb766-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb766-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb766-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb766-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb766-106">Добавляет (PIN) [вкладки](../resources/teamstab.md) для указанного [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fb766-106">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="fb766-107">Соответствующие приложения уже должен быть [установлен в группе](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="fb766-107">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb766-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb766-108">Permissions</span></span>
<span data-ttu-id="fb766-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb766-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb766-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb766-111">Permission type</span></span>      | <span data-ttu-id="fb766-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb766-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb766-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb766-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fb766-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb766-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb766-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb766-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb766-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb766-116">Not supported.</span></span>    |
| <span data-ttu-id="fb766-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb766-117">Application</span></span>                            | <span data-ttu-id="fb766-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb766-118">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="fb766-119">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="fb766-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fb766-120">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="fb766-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb766-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb766-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="fb766-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb766-122">Request headers</span></span>
| <span data-ttu-id="fb766-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb766-123">Header</span></span>       | <span data-ttu-id="fb766-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fb766-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb766-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb766-125">Authorization</span></span>  | <span data-ttu-id="fb766-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb766-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb766-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb766-128">Request body</span></span>

<span data-ttu-id="fb766-129">[TeamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="fb766-129">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="fb766-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb766-130">Response</span></span>

<span data-ttu-id="fb766-131">В случае успешного выполнения этот метод возвращает код отклика `201 OK`.</span><span class="sxs-lookup"><span data-stu-id="fb766-131">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb766-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fb766-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fb766-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb766-133">Request</span></span>

<span data-ttu-id="fb766-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb766-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="fb766-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb766-135">Response</span></span>

<span data-ttu-id="fb766-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fb766-136">The following is an example of the response.</span></span> <span data-ttu-id="fb766-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fb766-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fb766-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb766-138">All of the properties will be returned from an actual call.</span></span>
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
  "name": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="fb766-139">См. также</span><span class="sxs-lookup"><span data-stu-id="fb766-139">See also</span></span>

[<span data-ttu-id="fb766-140">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="fb766-140">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
