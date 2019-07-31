---
title: Обновление вкладки
description: Обновление свойств указанной вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 43d698e300cb4a9f2d9b6b094250fcbcd33d2821
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977473"
---
# <a name="update-tab"></a><span data-ttu-id="8aa7d-103">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="8aa7d-103">Update tab</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa7d-104">Обновление свойств указанной [вкладки](../resources/teamstab.md). Это можно использовать для настройки контента вкладки.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aa7d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aa7d-105">Permissions</span></span>
<span data-ttu-id="8aa7d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aa7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8aa7d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aa7d-108">Permission type</span></span>      | <span data-ttu-id="8aa7d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8aa7d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aa7d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aa7d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8aa7d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aa7d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8aa7d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aa7d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aa7d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-113">Not supported.</span></span>    |
|<span data-ttu-id="8aa7d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8aa7d-114">Application</span></span>                            | <span data-ttu-id="8aa7d-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aa7d-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="8aa7d-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8aa7d-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8aa7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aa7d-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8aa7d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aa7d-119">Request headers</span></span>
| <span data-ttu-id="8aa7d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8aa7d-120">Header</span></span>       | <span data-ttu-id="8aa7d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8aa7d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8aa7d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8aa7d-122">Authorization</span></span>  | <span data-ttu-id="8aa7d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8aa7d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8aa7d-125">Content-Type</span></span>  | <span data-ttu-id="8aa7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8aa7d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8aa7d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8aa7d-127">Request body</span></span>
<span data-ttu-id="8aa7d-128">В тексте запроса добавьте представление объекта [Tab](../resources/teamstab.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8aa7d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aa7d-129">Response</span></span>

<span data-ttu-id="8aa7d-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8aa7d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8aa7d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8aa7d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aa7d-132">Request</span></span>
<span data-ttu-id="8aa7d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8aa7d-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="8aa7d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aa7d-134">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8aa7d-135">См. также</span><span class="sxs-lookup"><span data-stu-id="8aa7d-135">See also</span></span>

[<span data-ttu-id="8aa7d-136">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="8aa7d-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

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
