---
title: Создание connectedOrganization
description: Создание новой связаннойорганизации.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 00cac73ca31774a4b86a0df3db5b7c958e65e052
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437424"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="c4eaf-103">Создание connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="c4eaf-103">Create connectedOrganization</span></span>

<span data-ttu-id="c4eaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4eaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4eaf-105">Создание нового [объекта connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4eaf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4eaf-106">Permissions</span></span>

<span data-ttu-id="c4eaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4eaf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4eaf-109">Permission type</span></span>|<span data-ttu-id="c4eaf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="c4eaf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4eaf-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4eaf-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c4eaf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4eaf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-114">Not supported.</span></span> |
| <span data-ttu-id="c4eaf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4eaf-115">Application</span></span>                            | <span data-ttu-id="c4eaf-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4eaf-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4eaf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4eaf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="c4eaf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4eaf-118">Request headers</span></span>

|<span data-ttu-id="c4eaf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4eaf-119">Name</span></span>|<span data-ttu-id="c4eaf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4eaf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4eaf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4eaf-121">Authorization</span></span>|<span data-ttu-id="c4eaf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4eaf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4eaf-124">Content-Type</span></span>|<span data-ttu-id="c4eaf-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4eaf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4eaf-127">Request body</span></span>
<span data-ttu-id="c4eaf-128">В теле запроса поставляем представление JSON объекта [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="c4eaf-129">В следующей таблице показаны свойства, необходимые при создании [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="c4eaf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4eaf-130">Property</span></span>|<span data-ttu-id="c4eaf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4eaf-131">Type</span></span>|<span data-ttu-id="c4eaf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4eaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4eaf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c4eaf-133">displayName</span></span>|<span data-ttu-id="c4eaf-134">String</span><span class="sxs-lookup"><span data-stu-id="c4eaf-134">String</span></span>|<span data-ttu-id="c4eaf-135">Имя подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-135">The connected organization name.</span></span> |
|<span data-ttu-id="c4eaf-136">description</span><span class="sxs-lookup"><span data-stu-id="c4eaf-136">description</span></span>|<span data-ttu-id="c4eaf-137">String</span><span class="sxs-lookup"><span data-stu-id="c4eaf-137">String</span></span>|<span data-ttu-id="c4eaf-138">Описание подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-138">The connected organization description.</span></span>|
|<span data-ttu-id="c4eaf-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="c4eaf-139">identitySources</span></span>|<span data-ttu-id="c4eaf-140">[коллекция identitySource](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="c4eaf-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="c4eaf-141">Коллекция с одним элементом, исходный источник удостоверений в этой связанной организации.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-141">A collection with one element, the initial identity source in this connected organization.</span></span>|
|<span data-ttu-id="c4eaf-142">state</span><span class="sxs-lookup"><span data-stu-id="c4eaf-142">state</span></span>|<span data-ttu-id="c4eaf-143">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="c4eaf-143">connectedOrganizationState</span></span>|<span data-ttu-id="c4eaf-144">Состояние связанной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запроса.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-144">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="c4eaf-145">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-145">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="c4eaf-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4eaf-146">Response</span></span>

<span data-ttu-id="c4eaf-147">В случае успешной работы этот метод возвращает код отклика и `201 Created` новый [объект connectedOrganization](../resources/connectedorganization.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-147">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4eaf-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4eaf-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4eaf-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4eaf-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4eaf-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4eaf-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4eaf-151">C#</span><span class="sxs-lookup"><span data-stu-id="c4eaf-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectedorganization-from-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4eaf-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4eaf-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectedorganization-from-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4eaf-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4eaf-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectedorganization-from-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4eaf-154">Java</span><span class="sxs-lookup"><span data-stu-id="c4eaf-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectedorganization-from-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4eaf-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4eaf-155">Response</span></span>
<span data-ttu-id="c4eaf-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4eaf-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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


