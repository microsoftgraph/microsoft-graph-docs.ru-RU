---
title: Вкладка "обновления"
description: Обновляет свойства указанной вкладки.
ms.openlocfilehash: 6943e9ea4ff602b3fcd4dc8ac899d55cee120ecc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076395"
---
# <a name="update-tab"></a><span data-ttu-id="850ef-103">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="850ef-103">Update tab</span></span>

> <span data-ttu-id="850ef-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="850ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="850ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="850ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="850ef-106">Обновляет свойства указанной [вкладки](../resources/teamstab.md). Это можно использовать для настройки содержимого вкладки.</span><span class="sxs-lookup"><span data-stu-id="850ef-106">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="850ef-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="850ef-107">Permissions</span></span>
<span data-ttu-id="850ef-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="850ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="850ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="850ef-110">Permission type</span></span>      | <span data-ttu-id="850ef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="850ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="850ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="850ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="850ef-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850ef-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="850ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="850ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="850ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="850ef-115">Not supported.</span></span>    |
|<span data-ttu-id="850ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="850ef-116">Application</span></span>                            | <span data-ttu-id="850ef-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850ef-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="850ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="850ef-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="850ef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="850ef-119">Request headers</span></span>
| <span data-ttu-id="850ef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="850ef-120">Header</span></span>       | <span data-ttu-id="850ef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="850ef-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="850ef-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="850ef-122">Authorization</span></span>  | <span data-ttu-id="850ef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="850ef-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="850ef-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="850ef-125">Content-Type</span></span>  | <span data-ttu-id="850ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="850ef-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="850ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="850ef-127">Request body</span></span>
<span data-ttu-id="850ef-128">В тексте запроса укажите представление JSON объекта [вкладки](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="850ef-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="850ef-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="850ef-129">Response</span></span>

<span data-ttu-id="850ef-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="850ef-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="850ef-131">Пример</span><span class="sxs-lookup"><span data-stu-id="850ef-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="850ef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="850ef-132">Request</span></span>
<span data-ttu-id="850ef-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="850ef-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="850ef-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="850ef-134">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="850ef-135">См. также</span><span class="sxs-lookup"><span data-stu-id="850ef-135">See also</span></span>

[<span data-ttu-id="850ef-136">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="850ef-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
