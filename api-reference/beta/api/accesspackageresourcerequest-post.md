---
title: Создание accessPackageResourceRequest
description: Создание нового accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f4cec8ead5d678e937b2648089593950fb104ff5
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401008"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="d4373-103">Создание accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="d4373-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="d4373-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4373-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4373-105">Создайте новый [объект accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) для запроса добавления ресурса в каталог пакетов доступа или удаления ресурса из каталога.</span><span class="sxs-lookup"><span data-stu-id="d4373-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>  <span data-ttu-id="d4373-106">Ресурс должен быть включен в каталог пакетов доступа, прежде чем роль этого ресурса может быть добавлена в пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="d4373-106">A resource must be included in an access package catalog before the role of that resource can be added to an access package.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4373-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4373-107">Permissions</span></span>

<span data-ttu-id="d4373-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4373-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4373-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4373-110">Permission type</span></span>                        | <span data-ttu-id="d4373-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4373-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4373-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4373-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4373-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4373-113">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="d4373-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4373-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4373-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4373-115">Not supported.</span></span> |
| <span data-ttu-id="d4373-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4373-116">Application</span></span>                            | <span data-ttu-id="d4373-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4373-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4373-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4373-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="d4373-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4373-119">Request headers</span></span>

| <span data-ttu-id="d4373-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d4373-120">Name</span></span>          | <span data-ttu-id="d4373-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d4373-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d4373-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4373-122">Authorization</span></span> | <span data-ttu-id="d4373-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4373-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4373-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4373-125">Content-Type</span></span>  | <span data-ttu-id="d4373-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4373-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4373-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4373-128">Request body</span></span>

<span data-ttu-id="d4373-129">В теле запроса поставляем представление JSON объекта [accessPackageResourceRequest.](../resources/accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="d4373-129">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="d4373-130">`accessPackageResource`Включайте связь с [объектом accessPackageResource](../resources/accesspackageresource.md) в качестве части запроса.</span><span class="sxs-lookup"><span data-stu-id="d4373-130">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="d4373-131">Чтобы добавить группу Azure AD в качестве  ресурса в каталог, задайте каталогId ID каталога, **requestType** to be `AdminAdd` и `accessPackageResource` представляющий ресурс.</span><span class="sxs-lookup"><span data-stu-id="d4373-131">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="d4373-132">Значение свойства **originSystem** внутри должно быть, а значение originId — `accessPackageResource` `AadGroup` идентификатор группы. </span><span class="sxs-lookup"><span data-stu-id="d4373-132">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="d4373-133">Чтобы удалить приложение Azure AD из  каталога, установите каталогId в ID каталога, **requestType** to be и объект ресурса, который необходимо `AdminRemove` `accessPackageResource` удалить.</span><span class="sxs-lookup"><span data-stu-id="d4373-133">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="d4373-134">Объект ресурса можно получить с помощью [списка accessPackageResources.](accesspackagecatalog-list-accesspackageresources.md)</span><span class="sxs-lookup"><span data-stu-id="d4373-134">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="d4373-135">Чтобы назначить среду геолокации для ресурса Sharepoint Online с несколькими геолокациями, включите связь **accessPackageResourceEnvironment** в `accessPackageResource` объекте.</span><span class="sxs-lookup"><span data-stu-id="d4373-135">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="d4373-136">Это можно сделать двумя способами:</span><span class="sxs-lookup"><span data-stu-id="d4373-136">This can be done in two ways:</span></span>
+ <span data-ttu-id="d4373-137">Чтобы `@odata.bind` назначить объекту `id` аннотацию, `accessPackageResourceEnvironment` используйте `accessPackageResourceEnvironment` аннотацию.</span><span class="sxs-lookup"><span data-stu-id="d4373-137">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="d4373-138">Укажите `originId` параметр `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` объекта.</span><span class="sxs-lookup"><span data-stu-id="d4373-138">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="d4373-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4373-139">Response</span></span>

<span data-ttu-id="d4373-140">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d4373-140">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4373-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4373-141">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource"></a><span data-ttu-id="d4373-142">Пример 1. Создание accessPackageResourceRequest для добавления сайта в качестве ресурса</span><span class="sxs-lookup"><span data-stu-id="d4373-142">Example 1: Create an accessPackageResourceRequest for adding a site as a resource</span></span>

#### <a name="request"></a><span data-ttu-id="d4373-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4373-143">Request</span></span>

<span data-ttu-id="d4373-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4373-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4373-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4373-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4373-146">C#</span><span class="sxs-lookup"><span data-stu-id="d4373-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4373-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4373-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4373-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4373-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4373-149">Java</span><span class="sxs-lookup"><span data-stu-id="d4373-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4373-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4373-150">Response</span></span>

<span data-ttu-id="d4373-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4373-151">The following is an example of the response.</span></span>

> <span data-ttu-id="d4373-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d4373-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="d4373-153">Пример 2. Создание accessPackageResourceRequest для добавления сайта в качестве ресурса и назначение accessPackageResourceEnvironment с помощью @odata.bind</span><span class="sxs-lookup"><span data-stu-id="d4373-153">Example 2: Create an accessPackageResourceRequest for adding a site as a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="d4373-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4373-154">Request</span></span>

<span data-ttu-id="d4373-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4373-155">The following is an example of the request.</span></span> <span data-ttu-id="d4373-156">В этом примере аннотация используется для назначения `@odata.bind` `id` `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` объекта.</span><span class="sxs-lookup"><span data-stu-id="d4373-156">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="d4373-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4373-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4373-158">C#</span><span class="sxs-lookup"><span data-stu-id="d4373-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4373-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4373-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4373-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4373-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4373-161">Java</span><span class="sxs-lookup"><span data-stu-id="d4373-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4373-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4373-162">Response</span></span>

<span data-ttu-id="d4373-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4373-163">The following is an example of the response.</span></span>

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

### <a name="example-3-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="d4373-164">Пример 3. Создание accessPackageResourceRequest для добавления сайта в качестве ресурса и назначение accessPackageResourceEnvironment с помощью originId</span><span class="sxs-lookup"><span data-stu-id="d4373-164">Example 3: Create an accessPackageResourceRequest for adding a site as a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="d4373-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4373-165">Request</span></span>

<span data-ttu-id="d4373-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4373-166">The following is an example of the request.</span></span> <span data-ttu-id="d4373-167">В этом примере параметры объекта `accessPackageResourceEnvironment` указаны в `accessPackageResourceEnvironment` объекте.</span><span class="sxs-lookup"><span data-stu-id="d4373-167">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="d4373-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4373-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4373-169">C#</span><span class="sxs-lookup"><span data-stu-id="d4373-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4373-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4373-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4373-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4373-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4373-172">Java</span><span class="sxs-lookup"><span data-stu-id="d4373-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4373-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4373-173">Response</span></span>

<span data-ttu-id="d4373-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4373-174">The following is an example of the response.</span></span>

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

### <a name="example-4-create-an-accesspackageresourcerequest-for-adding-a-group-as-a-resource"></a><span data-ttu-id="d4373-175">Пример 4. Создание accessPackageResourceRequest для добавления группы в качестве ресурса</span><span class="sxs-lookup"><span data-stu-id="d4373-175">Example 4: Create an accessPackageResourceRequest for adding a group as a resource</span></span>

#### <a name="request"></a><span data-ttu-id="d4373-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4373-176">Request</span></span>

<span data-ttu-id="d4373-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4373-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests4"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{

  "catalogId":"beedadfe-01d5-4025-910b-84abb9369997",
  "requestType": "AdminAdd",
  "accessPackageResource": {
     "originId": "c6294667-7348-4f5a-be73-9d2c65f574f3",
     "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="d4373-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4373-178">Response</span></span>

<span data-ttu-id="d4373-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4373-179">The following is an example of the response.</span></span>

> <span data-ttu-id="d4373-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d4373-180">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "id": "acc2294e-f37f-42d3-981d-4e83847ed0ce",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled"
}
```

### <a name="example-5-create-an-accesspackageresourcerequest-for-removing-a-resource"></a><span data-ttu-id="d4373-181">Пример 5. Создание accessPackageResourceRequest для удаления ресурса</span><span class="sxs-lookup"><span data-stu-id="d4373-181">Example 5: Create an accessPackageResourceRequest for removing a resource</span></span>

#### <a name="request"></a><span data-ttu-id="d4373-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4373-182">Request</span></span>

<span data-ttu-id="d4373-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4373-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests5"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "requestType": "AdminRemove",
  "accessPackageResource": {
    "id": "354078e5-dbce-4894-8af4-0ab274d41662"
  }
}

```

#### <a name="response"></a><span data-ttu-id="d4373-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4373-184">Response</span></span>

<span data-ttu-id="d4373-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4373-185">The following is an example of the response.</span></span>

> <span data-ttu-id="d4373-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d4373-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "id": "65c3340d-defb-49a9-8930-63841fda0e68",
  "requestType": "AdminRemove",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled"
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
