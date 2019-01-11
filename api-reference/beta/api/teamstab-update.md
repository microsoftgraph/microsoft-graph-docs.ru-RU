---
title: Вкладка "обновления"
description: Обновляет свойства указанной вкладки.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c17381432465ae318d86a818922d161ab46e762f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815066"
---
# <a name="update-tab"></a><span data-ttu-id="0278c-103">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="0278c-103">Update tab</span></span>

> <span data-ttu-id="0278c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0278c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0278c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0278c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0278c-106">Обновляет свойства указанной [вкладки](../resources/teamstab.md). Это можно использовать для настройки содержимого вкладки.</span><span class="sxs-lookup"><span data-stu-id="0278c-106">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="0278c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0278c-107">Permissions</span></span>
<span data-ttu-id="0278c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0278c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0278c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0278c-110">Permission type</span></span>      | <span data-ttu-id="0278c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0278c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0278c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0278c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0278c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0278c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0278c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0278c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0278c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0278c-115">Not supported.</span></span>    |
|<span data-ttu-id="0278c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0278c-116">Application</span></span>                            | <span data-ttu-id="0278c-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0278c-117">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="0278c-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="0278c-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0278c-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="0278c-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0278c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0278c-120">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0278c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0278c-121">Request headers</span></span>
| <span data-ttu-id="0278c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0278c-122">Header</span></span>       | <span data-ttu-id="0278c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0278c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0278c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0278c-124">Authorization</span></span>  | <span data-ttu-id="0278c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0278c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0278c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0278c-127">Content-Type</span></span>  | <span data-ttu-id="0278c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0278c-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0278c-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0278c-129">Request body</span></span>
<span data-ttu-id="0278c-130">В тексте запроса укажите представление JSON объекта [вкладки](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="0278c-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0278c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0278c-131">Response</span></span>

<span data-ttu-id="0278c-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0278c-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0278c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0278c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0278c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0278c-134">Request</span></span>
<span data-ttu-id="0278c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0278c-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="0278c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0278c-136">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="0278c-137">См. также</span><span class="sxs-lookup"><span data-stu-id="0278c-137">See also</span></span>

[<span data-ttu-id="0278c-138">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="0278c-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
