---
title: Обновление объекта команды
description: Обновление свойств указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 30467e6103dbc858e0b42de7012e9c2171f7372a
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848782"
---
# <a name="update-team"></a><span data-ttu-id="6b631-103">Обновление объекта команды</span><span class="sxs-lookup"><span data-stu-id="6b631-103">Update team</span></span>

<span data-ttu-id="6b631-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b631-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6b631-105">Обновление свойств указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="6b631-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b631-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b631-106">Permissions</span></span>
<span data-ttu-id="6b631-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6b631-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b631-109">Permission type</span></span>      | <span data-ttu-id="6b631-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b631-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b631-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b631-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b631-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b631-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6b631-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b631-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b631-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b631-114">Not supported.</span></span>    |
|<span data-ttu-id="6b631-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b631-115">Application</span></span> | <span data-ttu-id="6b631-116">Теамсеттингс. ReadWrite. Group \*, Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6b631-116">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="6b631-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6b631-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="6b631-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6b631-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="6b631-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="6b631-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b631-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b631-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6b631-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b631-121">Request headers</span></span>
| <span data-ttu-id="6b631-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b631-122">Header</span></span>       | <span data-ttu-id="6b631-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6b631-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b631-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b631-124">Authorization</span></span>  | <span data-ttu-id="6b631-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b631-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b631-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b631-127">Content-Type</span></span>  | <span data-ttu-id="6b631-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6b631-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b631-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b631-129">Request body</span></span>
<span data-ttu-id="6b631-130">В тексте запроса добавьте представление объекта [группы](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b631-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b631-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b631-131">Response</span></span>

<span data-ttu-id="6b631-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6b631-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6b631-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6b631-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6b631-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b631-134">Request</span></span>
<span data-ttu-id="6b631-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b631-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b631-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b631-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6b631-137">C#</span><span class="sxs-lookup"><span data-stu-id="6b631-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b631-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b631-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b631-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b631-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b631-140">Java</span><span class="sxs-lookup"><span data-stu-id="6b631-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6b631-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b631-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

