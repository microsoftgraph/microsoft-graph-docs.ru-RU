---
title: Вкладка "обновления"
description: Обновляет свойства указанной вкладки.
ms.openlocfilehash: fb2346fbadcb9794e05f8bb583596536a5710052
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027575"
---
# <a name="update-tab"></a><span data-ttu-id="f7719-103">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="f7719-103">Update tab</span></span>



<span data-ttu-id="f7719-104">Обновляет свойства указанной [вкладки](../resources/teamstab.md). Это можно использовать для настройки содержимого вкладки.</span><span class="sxs-lookup"><span data-stu-id="f7719-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7719-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7719-105">Permissions</span></span>
<span data-ttu-id="f7719-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f7719-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7719-108">Permission type</span></span>      | <span data-ttu-id="f7719-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7719-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7719-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7719-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7719-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7719-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7719-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7719-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7719-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7719-113">Not supported.</span></span>    |
|<span data-ttu-id="f7719-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7719-114">Application</span></span>                            | <span data-ttu-id="f7719-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7719-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f7719-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7719-116">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f7719-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7719-117">Request headers</span></span>
| <span data-ttu-id="f7719-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7719-118">Header</span></span>       | <span data-ttu-id="f7719-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f7719-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7719-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7719-120">Authorization</span></span>  | <span data-ttu-id="f7719-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7719-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7719-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7719-123">Content-Type</span></span>  | <span data-ttu-id="f7719-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7719-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7719-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7719-125">Request body</span></span>
<span data-ttu-id="f7719-126">В тексте запроса укажите представление JSON объекта [вкладки](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="f7719-126">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f7719-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7719-127">Response</span></span>

<span data-ttu-id="f7719-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7719-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7719-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f7719-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7719-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7719-130">Request</span></span>
<span data-ttu-id="f7719-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7719-131">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="f7719-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7719-132">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f7719-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f7719-133">See also</span></span>

[<span data-ttu-id="f7719-134">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="f7719-134">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
