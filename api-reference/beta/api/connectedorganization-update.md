---
title: Обновление объекта Коннектедорганизатион
description: Обновление объекта Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 804beb5db6fe42d430912fc14377764b9f4d6dcb
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566518"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="5c966-103">Обновление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5c966-103">Update connectedOrganization</span></span>

<span data-ttu-id="5c966-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c966-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c966-105">Обновление объекта [коннектедорганизатион](../resources/connectedorganization.md) для изменения одного или нескольких его свойств.</span><span class="sxs-lookup"><span data-stu-id="5c966-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c966-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c966-106">Permissions</span></span>
<span data-ttu-id="5c966-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c966-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c966-109">Permission type</span></span>|<span data-ttu-id="5c966-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c966-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c966-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c966-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c966-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c966-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="5c966-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c966-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c966-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c966-114">Not supported.</span></span> |
|<span data-ttu-id="5c966-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c966-115">Application</span></span>                            | <span data-ttu-id="5c966-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c966-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c966-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c966-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5c966-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c966-118">Request headers</span></span>
|<span data-ttu-id="5c966-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c966-119">Name</span></span>|<span data-ttu-id="5c966-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c966-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c966-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c966-121">Authorization</span></span>|<span data-ttu-id="5c966-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c966-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5c966-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c966-124">Content-Type</span></span>|<span data-ttu-id="5c966-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c966-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c966-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c966-127">Request body</span></span>
<span data-ttu-id="5c966-128">В тексте запроса добавьте представление объекта [коннектедорганизатион](../resources/connectedorganization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c966-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="5c966-129">В следующей таблице приведены свойства, необходимые при обновлении [коннектедорганизатион](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="5c966-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="5c966-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c966-130">Property</span></span>|<span data-ttu-id="5c966-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5c966-131">Type</span></span>|<span data-ttu-id="5c966-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5c966-132">Description</span></span>|
|:---|:---|:---|
| `displayName`  |`String` | <span data-ttu-id="5c966-133">Имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="5c966-133">The connected organization name.</span></span>  |
| `description`  |`String` | <span data-ttu-id="5c966-134">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="5c966-134">The connected organization description.</span></span> |

## <a name="response"></a><span data-ttu-id="5c966-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c966-135">Response</span></span>

<span data-ttu-id="5c966-136">В случае успешного выполнения этот метод возвращает `204 Accepted` код отклика и объект [коннектедорганизатион](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c966-136">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c966-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c966-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c966-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c966-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5c966-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c966-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectedorganization"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization new name",
  "description":"Connected organization new description"
}
```
# <a name="c"></a>[<span data-ttu-id="5c966-140">C#</span><span class="sxs-lookup"><span data-stu-id="5c966-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c966-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c966-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c966-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c966-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5c966-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c966-143">Response</span></span>
<span data-ttu-id="5c966-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c966-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 204 Accepted
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization new name",
  "description":"Connected organization new description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
