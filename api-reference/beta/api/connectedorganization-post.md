---
title: Создание connectedOrganization
description: Создание новой связаннойорганизации.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 284a7e4c907fb5305eee06b124250467fc27b450
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896286"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="9d304-103">Создание connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="9d304-103">Create connectedOrganization</span></span>

<span data-ttu-id="9d304-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d304-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d304-105">Создание нового [объекта connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="9d304-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d304-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d304-106">Permissions</span></span>

<span data-ttu-id="9d304-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d304-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d304-109">Permission type</span></span>|<span data-ttu-id="9d304-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d304-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="9d304-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d304-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d304-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d304-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9d304-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d304-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d304-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d304-114">Not supported.</span></span> |
| <span data-ttu-id="9d304-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9d304-115">Application</span></span>                            | <span data-ttu-id="9d304-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d304-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d304-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d304-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="9d304-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d304-118">Request headers</span></span>

|<span data-ttu-id="9d304-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9d304-119">Name</span></span>|<span data-ttu-id="9d304-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9d304-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d304-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d304-121">Authorization</span></span>|<span data-ttu-id="9d304-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d304-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d304-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d304-124">Content-Type</span></span>|<span data-ttu-id="9d304-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d304-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d304-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d304-127">Request body</span></span>
<span data-ttu-id="9d304-128">В теле запроса поставляем представление JSON объекта [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="9d304-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="9d304-129">В следующей таблице показаны свойства, необходимые при создании [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="9d304-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="9d304-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d304-130">Property</span></span>|<span data-ttu-id="9d304-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d304-131">Type</span></span>|<span data-ttu-id="9d304-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d304-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d304-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9d304-133">displayName</span></span>|<span data-ttu-id="9d304-134">String</span><span class="sxs-lookup"><span data-stu-id="9d304-134">String</span></span>|<span data-ttu-id="9d304-135">Имя подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="9d304-135">The connected organization name.</span></span> |
|<span data-ttu-id="9d304-136">description</span><span class="sxs-lookup"><span data-stu-id="9d304-136">description</span></span>|<span data-ttu-id="9d304-137">String</span><span class="sxs-lookup"><span data-stu-id="9d304-137">String</span></span>|<span data-ttu-id="9d304-138">Описание подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="9d304-138">The connected organization description.</span></span>|
|<span data-ttu-id="9d304-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="9d304-139">identitySources</span></span>|<span data-ttu-id="9d304-140">[коллекция identitySource](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="9d304-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="9d304-141">Коллекция с одним элементом, исходный источник удостоверений в этой связанной организации.</span><span class="sxs-lookup"><span data-stu-id="9d304-141">A collection with one element, the initial identity source in this connected organization.</span></span>|
|<span data-ttu-id="9d304-142">state</span><span class="sxs-lookup"><span data-stu-id="9d304-142">state</span></span>|<span data-ttu-id="9d304-143">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="9d304-143">connectedOrganizationState</span></span>|<span data-ttu-id="9d304-144">Состояние связанной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запроса.</span><span class="sxs-lookup"><span data-stu-id="9d304-144">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="9d304-145">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="9d304-145">Possible values are: `configured`, `proposed`.</span></span>|

<span data-ttu-id="9d304-146">Один член коллекции identitySources должен быть как типа [domainIdentitySource,](../resources/domainidentitysource.md) так и [externalDomainFederation.](../resources/externaldomainfederation.md)</span><span class="sxs-lookup"><span data-stu-id="9d304-146">The single member of the identitySources collection should be of either the [domainIdentitySource](../resources/domainidentitysource.md) or [externalDomainFederation](../resources/externaldomainfederation.md) type.</span></span>  <span data-ttu-id="9d304-147">Если звонящая предоставляет domainIdentitySource, вызов является успешным, и домен соответствует зарегистрированным доменам клиента Azure Active Directory, после чего созданная подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](../resources/azureactivedirectorytenant.md)</span><span class="sxs-lookup"><span data-stu-id="9d304-147">If the caller provides a domainIdentitySource, the call is successful, and the domain corresponds to a registered domain of an Azure Active Directory tenant, then the resulting connectedOrganization that is created will have an identitySources collection containing a single member of the [azureActiveDirectoryTenant](../resources/azureactivedirectorytenant.md) type.</span></span>

## <a name="response"></a><span data-ttu-id="9d304-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d304-148">Response</span></span>

<span data-ttu-id="9d304-149">В случае успешной работы этот метод возвращает код отклика и `201 Created` новый [объект connectedOrganization](../resources/connectedorganization.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9d304-149">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d304-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="9d304-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d304-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d304-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9d304-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d304-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9d304-153">C#</span><span class="sxs-lookup"><span data-stu-id="9d304-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectedorganization-from-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d304-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d304-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectedorganization-from-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d304-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d304-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectedorganization-from-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d304-156">Java</span><span class="sxs-lookup"><span data-stu-id="9d304-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectedorganization-from-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d304-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d304-157">Response</span></span>
<span data-ttu-id="9d304-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d304-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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


