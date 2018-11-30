---
title: Добавление вкладки канала
description: 'Добавляет (PIN) вкладку для указанного канала в группе. '
ms.openlocfilehash: be246b0308be83e0b411fa89fe16034018756829
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076391"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="f3659-103">Добавление вкладки канала</span><span class="sxs-lookup"><span data-stu-id="f3659-103">Add tab to channel</span></span>

> <span data-ttu-id="f3659-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3659-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3659-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3659-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3659-106">Добавляет (PIN) [вкладки](../resources/teamstab.md) для указанного [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f3659-106">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="f3659-107">Соответствующие приложения уже должен быть [установлен в группе](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="f3659-107">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3659-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3659-108">Permissions</span></span>
<span data-ttu-id="f3659-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3659-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3659-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3659-111">Permission type</span></span>      | <span data-ttu-id="f3659-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3659-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3659-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3659-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f3659-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3659-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3659-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3659-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3659-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3659-116">Not supported.</span></span>    |
| <span data-ttu-id="f3659-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3659-117">Application</span></span>                            | <span data-ttu-id="f3659-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3659-118">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f3659-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3659-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="f3659-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3659-120">Request headers</span></span>
| <span data-ttu-id="f3659-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3659-121">Header</span></span>       | <span data-ttu-id="f3659-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3659-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3659-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3659-123">Authorization</span></span>  | <span data-ttu-id="f3659-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3659-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3659-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3659-126">Request body</span></span>

<span data-ttu-id="f3659-127">[TeamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="f3659-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="f3659-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3659-128">Response</span></span>

<span data-ttu-id="f3659-129">В случае успешного выполнения этот метод возвращает код отклика `201 OK`.</span><span class="sxs-lookup"><span data-stu-id="f3659-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3659-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f3659-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f3659-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3659-131">Request</span></span>

<span data-ttu-id="f3659-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3659-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="f3659-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3659-133">Response</span></span>

<span data-ttu-id="f3659-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f3659-134">The following is an example of the response.</span></span> <span data-ttu-id="f3659-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f3659-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f3659-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3659-136">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f3659-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f3659-137">See also</span></span>

[<span data-ttu-id="f3659-138">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="f3659-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
