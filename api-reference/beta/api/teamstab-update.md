---
title: Обновление вкладки
description: Обновление свойств указанной вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bdfcc21c0e078c20b04db2e9d5cce6247ac86aeb
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848342"
---
# <a name="update-tab"></a><span data-ttu-id="e77f2-103">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="e77f2-103">Update tab</span></span>

<span data-ttu-id="e77f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e77f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e77f2-105">Обновление свойств указанной [вкладки](../resources/teamstab.md). Это можно использовать для настройки контента вкладки.</span><span class="sxs-lookup"><span data-stu-id="e77f2-105">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="e77f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e77f2-106">Permissions</span></span>
<span data-ttu-id="e77f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e77f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e77f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e77f2-109">Permission type</span></span>      | <span data-ttu-id="e77f2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e77f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e77f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e77f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e77f2-112">TeamsTab. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e77f2-112">TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="e77f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e77f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e77f2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e77f2-114">Not supported.</span></span>    |
|<span data-ttu-id="e77f2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e77f2-115">Application</span></span>                            | <span data-ttu-id="e77f2-116">TeamsTab. ReadWrite. Group \*, TeamsTab. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e77f2-116">TeamsTab.ReadWrite.Group\*, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e77f2-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e77f2-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="e77f2-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e77f2-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="e77f2-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="e77f2-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e77f2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e77f2-120">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e77f2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e77f2-121">Request headers</span></span>
| <span data-ttu-id="e77f2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e77f2-122">Header</span></span>       | <span data-ttu-id="e77f2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e77f2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e77f2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e77f2-124">Authorization</span></span>  | <span data-ttu-id="e77f2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e77f2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e77f2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e77f2-127">Content-Type</span></span>  | <span data-ttu-id="e77f2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e77f2-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e77f2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e77f2-129">Request body</span></span>
<span data-ttu-id="e77f2-130">В тексте запроса добавьте представление объекта [Tab](../resources/teamstab.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e77f2-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e77f2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e77f2-131">Response</span></span>

<span data-ttu-id="e77f2-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e77f2-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e77f2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e77f2-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e77f2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e77f2-134">Request</span></span>
<span data-ttu-id="e77f2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e77f2-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="e77f2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e77f2-136">Response</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="e77f2-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e77f2-137">See also</span></span>

[<span data-ttu-id="e77f2-138">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="e77f2-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


