---
title: Создание accessPackageResourceRequest
description: Создайте новый accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e7ea15dbe0ec63e539246851ce853b83c40229aa
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934541"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="5525c-103">Создание accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="5525c-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="5525c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5525c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5525c-105">Создайте новый [объект accessPackageResourceRequest,](../resources/accesspackageresourcerequest.md) чтобы запросить добавление ресурса в каталог пакетов доступа или удаление ресурса из каталога.</span><span class="sxs-lookup"><span data-stu-id="5525c-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="5525c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5525c-106">Permissions</span></span>

<span data-ttu-id="5525c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5525c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5525c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5525c-109">Permission type</span></span>                        | <span data-ttu-id="5525c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5525c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5525c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5525c-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="5525c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5525c-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="5525c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5525c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5525c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5525c-114">Not supported.</span></span> |
| <span data-ttu-id="5525c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5525c-115">Application</span></span>                            | <span data-ttu-id="5525c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5525c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5525c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5525c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="5525c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5525c-118">Request headers</span></span>

| <span data-ttu-id="5525c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5525c-119">Name</span></span>          | <span data-ttu-id="5525c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5525c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5525c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5525c-121">Authorization</span></span> | <span data-ttu-id="5525c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5525c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5525c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5525c-124">Content-Type</span></span>  | <span data-ttu-id="5525c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5525c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5525c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5525c-127">Request body</span></span>

<span data-ttu-id="5525c-128">В теле запроса укажу представление объекта [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="5525c-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="5525c-129">`accessPackageResource`Включайте связь с [объектом accessPackageResource](../resources/accesspackageresource.md) как часть запроса.</span><span class="sxs-lookup"><span data-stu-id="5525c-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="5525c-130">Чтобы добавить группу Azure AD в качестве ресурса в каталог, задайте **catalogId** в качестве ИД каталога, **requestType** — в качестве `AdminAdd` `accessPackageResource` ресурса.</span><span class="sxs-lookup"><span data-stu-id="5525c-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="5525c-131">Значением свойства **originSystem** внутри должно быть, а `accessPackageResource` `AadGroup` **значением originId** является идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="5525c-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="5525c-132">Чтобы удалить приложение Azure AD из каталога, установите **catalogId** в качестве ИД каталога, **requestType** должен быть и объект ресурса, который `AdminRemove` необходимо `accessPackageResource` удалить.</span><span class="sxs-lookup"><span data-stu-id="5525c-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="5525c-133">Объект ресурса можно получить с помощью [списка accessPackageResources.](accesspackagecatalog-list-accesspackageresources.md)</span><span class="sxs-lookup"><span data-stu-id="5525c-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>


## <a name="response"></a><span data-ttu-id="5525c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5525c-134">Response</span></span>

<span data-ttu-id="5525c-135">В случае успеха этот метод возвращает код отклика серии 200 и новый [объект accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5525c-135">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5525c-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="5525c-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5525c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5525c-137">Request</span></span>

<span data-ttu-id="5525c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5525c-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5525c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5525c-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5525c-140">C#</span><span class="sxs-lookup"><span data-stu-id="5525c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5525c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5525c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5525c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5525c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5525c-143">Java</span><span class="sxs-lookup"><span data-stu-id="5525c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5525c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5525c-144">Response</span></span>

<span data-ttu-id="5525c-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5525c-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5525c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5525c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


