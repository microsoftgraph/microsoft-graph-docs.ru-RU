---
title: Создание Коннектедорганизатион
description: Создание нового Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0bdffc4bfb6a4c87ce3949dd76f4a87d673d707d
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566546"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="218d0-103">Создание Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="218d0-103">Create connectedOrganization</span></span>

<span data-ttu-id="218d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218d0-105">Создание нового объекта [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="218d0-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="218d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="218d0-106">Permissions</span></span>

<span data-ttu-id="218d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="218d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="218d0-109">Permission type</span></span>|<span data-ttu-id="218d0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="218d0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="218d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="218d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="218d0-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218d0-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="218d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="218d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218d0-114">Not supported.</span></span> |
| <span data-ttu-id="218d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="218d0-115">Application</span></span>                            | <span data-ttu-id="218d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="218d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="218d0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="218d0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="218d0-118">Request headers</span></span>

|<span data-ttu-id="218d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="218d0-119">Name</span></span>|<span data-ttu-id="218d0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="218d0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="218d0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="218d0-121">Authorization</span></span>|<span data-ttu-id="218d0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218d0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="218d0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="218d0-124">Content-Type</span></span>|<span data-ttu-id="218d0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218d0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="218d0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="218d0-127">Request body</span></span>
<span data-ttu-id="218d0-128">В тексте запроса добавьте представление объекта [коннектедорганизатион](../resources/connectedorganization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="218d0-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="218d0-129">В следующей таблице приведены свойства, необходимые при создании [коннектедорганизатион](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="218d0-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="218d0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="218d0-130">Property</span></span>|<span data-ttu-id="218d0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="218d0-131">Type</span></span>|<span data-ttu-id="218d0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="218d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="218d0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="218d0-133">displayName</span></span>|<span data-ttu-id="218d0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="218d0-134">String</span></span>|<span data-ttu-id="218d0-135">Имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="218d0-135">The connected organization name.</span></span> |
|<span data-ttu-id="218d0-136">description</span><span class="sxs-lookup"><span data-stu-id="218d0-136">description</span></span>|<span data-ttu-id="218d0-137">String</span><span class="sxs-lookup"><span data-stu-id="218d0-137">String</span></span>|<span data-ttu-id="218d0-138">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="218d0-138">The connected organization description.</span></span>|
|<span data-ttu-id="218d0-139">идентитисаурцес</span><span class="sxs-lookup"><span data-stu-id="218d0-139">identitySources</span></span>|<span data-ttu-id="218d0-140">Коллекция [идентитисаурце](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="218d0-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="218d0-141">Коллекция с одним элементом — начальным источником идентификаторов в этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="218d0-141">A collection with one element, the initial identity source in this connected organization.</span></span>|


## <a name="response"></a><span data-ttu-id="218d0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="218d0-142">Response</span></span>

<span data-ttu-id="218d0-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [коннектедорганизатион](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="218d0-143">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="218d0-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="218d0-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="218d0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="218d0-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="218d0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="218d0-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectedorganization_from_connectedorganizations"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.domainIdentitySource",
      "domainName": "example.com",
      "displayName": "example.com"
      }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="218d0-147">C#</span><span class="sxs-lookup"><span data-stu-id="218d0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectedorganization-from-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="218d0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="218d0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectedorganization-from-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="218d0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="218d0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectedorganization-from-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="218d0-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="218d0-150">Response</span></span>
<span data-ttu-id="218d0-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="218d0-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-06-08T20:13:53.7099947Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
