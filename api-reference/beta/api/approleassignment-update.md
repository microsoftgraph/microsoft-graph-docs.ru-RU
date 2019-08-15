---
title: Обновление объекта AppRoleAssignment
description: Обновление свойств объекта аппролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 34f01f3cf8d03158df41dfd74e17fd8f767244b8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408172"
---
# <a name="update-approleassignment"></a><span data-ttu-id="6f7ea-103">Обновление объекта AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6f7ea-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f7ea-104">Обновление свойств объекта аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f7ea-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f7ea-105">Permissions</span></span>
<span data-ttu-id="6f7ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f7ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f7ea-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f7ea-108">Permission type</span></span>      | <span data-ttu-id="6f7ea-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f7ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f7ea-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f7ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f7ea-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f7ea-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="6f7ea-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f7ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f7ea-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-113">Not supported.</span></span>    |
|<span data-ttu-id="6f7ea-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f7ea-114">Application</span></span> | <span data-ttu-id="6f7ea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f7ea-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f7ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6f7ea-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f7ea-117">Request headers</span></span>
| <span data-ttu-id="6f7ea-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6f7ea-118">Name</span></span>       | <span data-ttu-id="6f7ea-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6f7ea-119">Type</span></span> | <span data-ttu-id="6f7ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f7ea-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f7ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f7ea-121">Authorization</span></span>  | <span data-ttu-id="6f7ea-122">string</span><span class="sxs-lookup"><span data-stu-id="6f7ea-122">string</span></span>  | <span data-ttu-id="6f7ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f7ea-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f7ea-125">Request body</span></span>
<span data-ttu-id="6f7ea-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6f7ea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f7ea-129">Property</span></span>     | <span data-ttu-id="6f7ea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6f7ea-130">Type</span></span>   |<span data-ttu-id="6f7ea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6f7ea-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f7ea-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="6f7ea-132">creationTimestamp</span></span>|<span data-ttu-id="6f7ea-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f7ea-133">DateTimeOffset</span></span>|<span data-ttu-id="6f7ea-134">Время создания гранта.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="6f7ea-135">id</span><span class="sxs-lookup"><span data-stu-id="6f7ea-135">id</span></span>|<span data-ttu-id="6f7ea-136">GUID</span><span class="sxs-lookup"><span data-stu-id="6f7ea-136">Guid</span></span>|<span data-ttu-id="6f7ea-137">Идентификатор роли, назначенный субъекту.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="6f7ea-138">Эта роль должна быть объявлена в целевом приложении-ресурсе **resourceId** в свойстве **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="6f7ea-139">Если в ресурсе не объявлены разрешения, необходимо указать идентификатор по умолчанию (нулевой GUID).</span><span class="sxs-lookup"><span data-stu-id="6f7ea-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="6f7ea-140">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="6f7ea-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="6f7ea-141">principalDisplayName</span></span>|<span data-ttu-id="6f7ea-142">String</span><span class="sxs-lookup"><span data-stu-id="6f7ea-142">String</span></span>|<span data-ttu-id="6f7ea-143">Отображаемое имя субъекта, которому был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="6f7ea-144">principalId</span><span class="sxs-lookup"><span data-stu-id="6f7ea-144">principalId</span></span>|<span data-ttu-id="6f7ea-145">GUID</span><span class="sxs-lookup"><span data-stu-id="6f7ea-145">Guid</span></span>|<span data-ttu-id="6f7ea-146">Уникальный идентификатор (**ObjectID**) субъекта, которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="6f7ea-147">**Примечания**: обязательные.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="6f7ea-148">principalType</span><span class="sxs-lookup"><span data-stu-id="6f7ea-148">principalType</span></span>|<span data-ttu-id="6f7ea-149">String</span><span class="sxs-lookup"><span data-stu-id="6f7ea-149">String</span></span>|<span data-ttu-id="6f7ea-150">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-150">The type of principal.</span></span>  <span data-ttu-id="6f7ea-151">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="6f7ea-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="6f7ea-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6f7ea-152">resourceDisplayName</span></span>|<span data-ttu-id="6f7ea-153">String</span><span class="sxs-lookup"><span data-stu-id="6f7ea-153">String</span></span>|<span data-ttu-id="6f7ea-154">Отображаемое имя ресурса, для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="6f7ea-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="6f7ea-155">resourceId</span></span>|<span data-ttu-id="6f7ea-156">GUID</span><span class="sxs-lookup"><span data-stu-id="6f7ea-156">Guid</span></span>|<span data-ttu-id="6f7ea-157">Уникальный идентификатор (**ObjectID**) для целевого ресурса (субъекта-службы), для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="6f7ea-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f7ea-158">Response</span></span>

<span data-ttu-id="6f7ea-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f7ea-160">Пример</span><span class="sxs-lookup"><span data-stu-id="6f7ea-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f7ea-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f7ea-161">Request</span></span>
<span data-ttu-id="6f7ea-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6f7ea-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f7ea-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{id}
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f7ea-164">C#</span><span class="sxs-lookup"><span data-stu-id="6f7ea-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f7ea-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f7ea-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f7ea-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6f7ea-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f7ea-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f7ea-167">Response</span></span>
<span data-ttu-id="6f7ea-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f7ea-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
