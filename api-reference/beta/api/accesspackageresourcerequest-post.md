---
title: Создание accessPackageResourceRequest
description: Создание нового accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e0d85470f8217887364d8c37e760945205edec51
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048528"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="6cf04-103">Создание accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="6cf04-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="6cf04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cf04-105">Создайте новый [объект accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) для запроса добавления ресурса в каталог пакетов доступа или удаления ресурса из каталога.</span><span class="sxs-lookup"><span data-stu-id="6cf04-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cf04-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cf04-106">Permissions</span></span>

<span data-ttu-id="6cf04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cf04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cf04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cf04-109">Permission type</span></span>                        | <span data-ttu-id="6cf04-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cf04-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6cf04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cf04-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cf04-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf04-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="6cf04-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cf04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cf04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cf04-114">Not supported.</span></span> |
| <span data-ttu-id="6cf04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cf04-115">Application</span></span>                            | <span data-ttu-id="6cf04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cf04-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cf04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cf04-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="6cf04-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cf04-118">Request headers</span></span>

| <span data-ttu-id="6cf04-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6cf04-119">Name</span></span>          | <span data-ttu-id="6cf04-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6cf04-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6cf04-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cf04-121">Authorization</span></span> | <span data-ttu-id="6cf04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cf04-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cf04-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cf04-124">Content-Type</span></span>  | <span data-ttu-id="6cf04-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cf04-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cf04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cf04-127">Request body</span></span>

<span data-ttu-id="6cf04-128">В теле запроса поставляем представление JSON объекта [accessPackageResourceRequest.](../resources/accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6cf04-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="6cf04-129">`accessPackageResource`Включайте связь с [объектом accessPackageResource](../resources/accesspackageresource.md) в качестве части запроса.</span><span class="sxs-lookup"><span data-stu-id="6cf04-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="6cf04-130">Чтобы добавить группу Azure AD в качестве  ресурса в каталог, задайте каталогId ID каталога, **requestType** to be `AdminAdd` и `accessPackageResource` представляющий ресурс.</span><span class="sxs-lookup"><span data-stu-id="6cf04-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="6cf04-131">Значение свойства **originSystem** внутри должно быть, а значение originId — `accessPackageResource` `AadGroup` идентификатор группы. </span><span class="sxs-lookup"><span data-stu-id="6cf04-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="6cf04-132">Чтобы удалить приложение Azure AD из  каталога, установите каталогId в ID каталога, **requestType** to be и объект ресурса, который необходимо `AdminRemove` `accessPackageResource` удалить.</span><span class="sxs-lookup"><span data-stu-id="6cf04-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="6cf04-133">Объект ресурса можно получить с помощью [списка accessPackageResources.](accesspackagecatalog-list-accesspackageresources.md)</span><span class="sxs-lookup"><span data-stu-id="6cf04-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="6cf04-134">Чтобы назначить среду геолокации для ресурса Sharepoint Online с несколькими геолокациями, включите связь **accessPackageResourceEnvironment** в `accessPackageResource` объекте.</span><span class="sxs-lookup"><span data-stu-id="6cf04-134">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="6cf04-135">Это можно сделать двумя способами:</span><span class="sxs-lookup"><span data-stu-id="6cf04-135">This can be done in two ways:</span></span>
+ <span data-ttu-id="6cf04-136">Чтобы `@odata.bind` назначить объекту `id` аннотацию, `accessPackageResourceEnvironment` используйте `accessPackageResourceEnvironment` аннотацию.</span><span class="sxs-lookup"><span data-stu-id="6cf04-136">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="6cf04-137">Укажите `originId` параметр `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` объекта.</span><span class="sxs-lookup"><span data-stu-id="6cf04-137">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="6cf04-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf04-138">Response</span></span>

<span data-ttu-id="6cf04-139">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6cf04-139">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cf04-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6cf04-140">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest"></a><span data-ttu-id="6cf04-141">Пример 1. Создание accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="6cf04-141">Example 1: Create an accessPackageResourceRequest</span></span>

#### <a name="request"></a><span data-ttu-id="6cf04-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cf04-142">Request</span></span>

<span data-ttu-id="6cf04-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cf04-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6cf04-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf04-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
     "displayName": "Sales",
     "description": "https://contoso.sharepoint.com/sites/Sales",
     "url": "https://contoso.sharepoint.com/sites/Sales",
     "resourceType": "SharePoint Online Site",
     "originId": "https://contoso.sharepoint.com/sites/Sales",
     "originSystem": "SharePointOnline"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6cf04-145">C#</span><span class="sxs-lookup"><span data-stu-id="6cf04-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cf04-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cf04-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cf04-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cf04-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cf04-148">Java</span><span class="sxs-lookup"><span data-stu-id="6cf04-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cf04-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf04-149">Response</span></span>

<span data-ttu-id="6cf04-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6cf04-150">The following is an example of the response.</span></span>

> <span data-ttu-id="6cf04-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6cf04-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

### <a name="example-2-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="6cf04-152">Пример 2. Создание accessPackageResourceRequest для ресурса и назначение accessPackageResourceEnvironment с помощью @odata.bind</span><span class="sxs-lookup"><span data-stu-id="6cf04-152">Example 2: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="6cf04-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cf04-153">Request</span></span>

<span data-ttu-id="6cf04-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cf04-154">The following is an example of the request.</span></span> <span data-ttu-id="6cf04-155">В этом примере аннотация используется для назначения `@odata.bind` `id` `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` объекта.</span><span class="sxs-lookup"><span data-stu-id="6cf04-155">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="6cf04-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf04-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests_with_accessPackageResourceEnvironment"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "accessPackageResource": {
        "displayName": "Community Outreach",
        "description": "https://contoso.sharepoint.com/sites/CSR",
        "resourceType": "SharePoint Online Site",
        "originId": "https://contoso.sharepoint.com/sites/CSR",
        "originSystem": "SharePointOnline",
        "accessPackageResourceEnvironment@odata.bind": "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"
    },
    "requestType": "AdminAdd"
}
```
# <a name="c"></a>[<span data-ttu-id="6cf04-157">C#</span><span class="sxs-lookup"><span data-stu-id="6cf04-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cf04-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cf04-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cf04-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cf04-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cf04-160">Java</span><span class="sxs-lookup"><span data-stu-id="6cf04-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cf04-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf04-161">Response</span></span>

<span data-ttu-id="6cf04-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6cf04-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "executeImmediately": false,
    "id": "d3f800d5-0dd6-47f3-9e90-ef562c7551dc",
    "requestType": "AdminAdd",
    "requestState": "Delivered",
    "requestStatus": "Fulfilled",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="example-3-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="6cf04-163">Пример 3. Создание accessPackageResourceRequest для ресурса и назначение accessPackageResourceEnvironment с помощью originId</span><span class="sxs-lookup"><span data-stu-id="6cf04-163">Example 3: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="6cf04-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cf04-164">Request</span></span>

<span data-ttu-id="6cf04-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cf04-165">The following is an example of the request.</span></span> <span data-ttu-id="6cf04-166">В этом примере параметры объекта `accessPackageResourceEnvironment` указаны в `accessPackageResourceEnvironment` объекте.</span><span class="sxs-lookup"><span data-stu-id="6cf04-166">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="6cf04-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf04-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests_with_accessPackageResourceEnvironment_New"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "accessPackageResource": {
        "displayName": "Community Outreach",
        "description": "https://contoso.sharepoint.com/sites/CSR",
        "resourceType": "SharePoint Online Site",
        "originId": "https://contoso.sharepoint.com/sites/CSR",
        "originSystem": "SharePointOnline",
        "accessPackageResourceEnvironment": {
            "originId": "https://contoso-admin.sharepoint.com/"
        }
    },
    "requestType": "AdminAdd"
}
```
# <a name="c"></a>[<span data-ttu-id="6cf04-168">C#</span><span class="sxs-lookup"><span data-stu-id="6cf04-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cf04-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cf04-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cf04-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cf04-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cf04-171">Java</span><span class="sxs-lookup"><span data-stu-id="6cf04-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cf04-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf04-172">Response</span></span>

<span data-ttu-id="6cf04-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6cf04-173">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "executeImmediately": false,
    "id": "eadf3fbb-668c-4c3a-8d84-7c8bd73dc3e4",
    "requestType": "AdminAdd",
    "requestState": "Delivered",
    "requestStatus": "Fulfilled",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
