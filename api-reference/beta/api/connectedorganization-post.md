---
title: Создание connectedOrganization
description: Создайте новую connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75981889ae018e3c5852dae52bcb6ac09a195103
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872683"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="d6aff-103">Создание connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="d6aff-103">Create connectedOrganization</span></span>

<span data-ttu-id="d6aff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6aff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6aff-105">Создание объекта [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="d6aff-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6aff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6aff-106">Permissions</span></span>

<span data-ttu-id="d6aff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6aff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6aff-109">Permission type</span></span>|<span data-ttu-id="d6aff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6aff-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="d6aff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6aff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6aff-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6aff-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d6aff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6aff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6aff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6aff-114">Not supported.</span></span> |
| <span data-ttu-id="d6aff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6aff-115">Application</span></span>                            | <span data-ttu-id="d6aff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6aff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6aff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6aff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="d6aff-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6aff-118">Request headers</span></span>

|<span data-ttu-id="d6aff-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d6aff-119">Name</span></span>|<span data-ttu-id="d6aff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d6aff-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6aff-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6aff-121">Authorization</span></span>|<span data-ttu-id="d6aff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6aff-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6aff-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6aff-124">Content-Type</span></span>|<span data-ttu-id="d6aff-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6aff-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6aff-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6aff-127">Request body</span></span>
<span data-ttu-id="d6aff-128">В теле запроса укажу представление объекта [connectedOrganization](../resources/connectedorganization.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="d6aff-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="d6aff-129">В следующей таблице показаны свойства, необходимые при создании [объекта connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="d6aff-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="d6aff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6aff-130">Property</span></span>|<span data-ttu-id="d6aff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6aff-131">Type</span></span>|<span data-ttu-id="d6aff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6aff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6aff-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d6aff-133">displayName</span></span>|<span data-ttu-id="d6aff-134">String</span><span class="sxs-lookup"><span data-stu-id="d6aff-134">String</span></span>|<span data-ttu-id="d6aff-135">Имя подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="d6aff-135">The connected organization name.</span></span> |
|<span data-ttu-id="d6aff-136">description</span><span class="sxs-lookup"><span data-stu-id="d6aff-136">description</span></span>|<span data-ttu-id="d6aff-137">String</span><span class="sxs-lookup"><span data-stu-id="d6aff-137">String</span></span>|<span data-ttu-id="d6aff-138">Описание подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="d6aff-138">The connected organization description.</span></span>|
|<span data-ttu-id="d6aff-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="d6aff-139">identitySources</span></span>|<span data-ttu-id="d6aff-140">[Коллекция identitySource](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="d6aff-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="d6aff-141">Коллекция с одним элементом, исходным источником удостоверений в этой подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="d6aff-141">A collection with one element, the initial identity source in this connected organization.</span></span>|
|<span data-ttu-id="d6aff-142">state</span><span class="sxs-lookup"><span data-stu-id="d6aff-142">state</span></span>|<span data-ttu-id="d6aff-143">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="d6aff-143">connectedOrganizationState</span></span>|<span data-ttu-id="d6aff-144">Состояние подключенной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запросителя.</span><span class="sxs-lookup"><span data-stu-id="d6aff-144">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="d6aff-145">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="d6aff-145">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="d6aff-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6aff-146">Response</span></span>

<span data-ttu-id="d6aff-147">В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект connectedOrganization](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6aff-147">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6aff-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="d6aff-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6aff-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6aff-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6aff-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6aff-150">HTTP</span></span>](#tab/http)
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
  ],
  "state":"proposed"
}
```
# <a name="c"></a>[<span data-ttu-id="d6aff-151">C#</span><span class="sxs-lookup"><span data-stu-id="d6aff-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectedorganization-from-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6aff-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6aff-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectedorganization-from-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6aff-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6aff-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectedorganization-from-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6aff-154">Java</span><span class="sxs-lookup"><span data-stu-id="d6aff-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectedorganization-from-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6aff-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6aff-155">Response</span></span>
<span data-ttu-id="d6aff-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d6aff-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z",
  "state":"proposed"
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


