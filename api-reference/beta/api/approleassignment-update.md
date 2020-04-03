---
title: Обновление объекта AppRoleAssignment
description: Обновление свойств объекта аппролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 91a64bc0b4a31ef383332032a5ab9ed13b7f0e19
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123302"
---
# <a name="update-approleassignment"></a><span data-ttu-id="191b7-103">Обновление объекта AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="191b7-103">Update approleassignment</span></span>

<span data-ttu-id="191b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="191b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="191b7-105">Обновление свойств объекта аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="191b7-105">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="191b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="191b7-106">Permissions</span></span>
<span data-ttu-id="191b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="191b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="191b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="191b7-109">Permission type</span></span>      | <span data-ttu-id="191b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="191b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="191b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="191b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="191b7-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="191b7-112">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="191b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="191b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="191b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="191b7-114">Not supported.</span></span>    |
|<span data-ttu-id="191b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="191b7-115">Application</span></span> | <span data-ttu-id="191b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="191b7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="191b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="191b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="191b7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="191b7-118">Request headers</span></span>
| <span data-ttu-id="191b7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="191b7-119">Name</span></span>       | <span data-ttu-id="191b7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="191b7-120">Type</span></span> | <span data-ttu-id="191b7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="191b7-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="191b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="191b7-122">Authorization</span></span>  | <span data-ttu-id="191b7-123">string</span><span class="sxs-lookup"><span data-stu-id="191b7-123">string</span></span>  | <span data-ttu-id="191b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="191b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="191b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="191b7-126">Request body</span></span>
<span data-ttu-id="191b7-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="191b7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="191b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="191b7-130">Property</span></span>     | <span data-ttu-id="191b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="191b7-131">Type</span></span>   |<span data-ttu-id="191b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="191b7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="191b7-133">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="191b7-133">creationTimestamp</span></span>|<span data-ttu-id="191b7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="191b7-134">DateTimeOffset</span></span>|<span data-ttu-id="191b7-135">Время создания гранта.</span><span class="sxs-lookup"><span data-stu-id="191b7-135">The time when the grant was created.</span></span>|
|<span data-ttu-id="191b7-136">id</span><span class="sxs-lookup"><span data-stu-id="191b7-136">id</span></span>|<span data-ttu-id="191b7-137">GUID</span><span class="sxs-lookup"><span data-stu-id="191b7-137">Guid</span></span>|<span data-ttu-id="191b7-138">Идентификатор роли, назначенный субъекту.</span><span class="sxs-lookup"><span data-stu-id="191b7-138">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="191b7-139">Эта роль должна быть объявлена в целевом приложении-ресурсе **resourceId** в свойстве **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="191b7-139">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="191b7-140">Если в ресурсе не объявлены разрешения, необходимо указать идентификатор по умолчанию (нулевой GUID).</span><span class="sxs-lookup"><span data-stu-id="191b7-140">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="191b7-141">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="191b7-141">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="191b7-142">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="191b7-142">principalDisplayName</span></span>|<span data-ttu-id="191b7-143">String</span><span class="sxs-lookup"><span data-stu-id="191b7-143">String</span></span>|<span data-ttu-id="191b7-144">Отображаемое имя субъекта, которому был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="191b7-144">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="191b7-145">principalId</span><span class="sxs-lookup"><span data-stu-id="191b7-145">principalId</span></span>|<span data-ttu-id="191b7-146">GUID</span><span class="sxs-lookup"><span data-stu-id="191b7-146">Guid</span></span>|<span data-ttu-id="191b7-147">Уникальный идентификатор (**ObjectID**) субъекта, которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="191b7-147">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="191b7-148">**Примечания**: обязательные.</span><span class="sxs-lookup"><span data-stu-id="191b7-148">**Notes**: required.</span></span>            |
|<span data-ttu-id="191b7-149">principalType</span><span class="sxs-lookup"><span data-stu-id="191b7-149">principalType</span></span>|<span data-ttu-id="191b7-150">String</span><span class="sxs-lookup"><span data-stu-id="191b7-150">String</span></span>|<span data-ttu-id="191b7-151">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="191b7-151">The type of principal.</span></span>  <span data-ttu-id="191b7-152">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="191b7-152">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="191b7-153">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="191b7-153">resourceDisplayName</span></span>|<span data-ttu-id="191b7-154">String</span><span class="sxs-lookup"><span data-stu-id="191b7-154">String</span></span>|<span data-ttu-id="191b7-155">Отображаемое имя ресурса, для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="191b7-155">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="191b7-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="191b7-156">resourceId</span></span>|<span data-ttu-id="191b7-157">GUID</span><span class="sxs-lookup"><span data-stu-id="191b7-157">Guid</span></span>|<span data-ttu-id="191b7-158">Уникальный идентификатор (**ObjectID**) для целевого ресурса (субъекта-службы), для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="191b7-158">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="191b7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="191b7-159">Response</span></span>

<span data-ttu-id="191b7-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="191b7-160">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="191b7-161">Пример</span><span class="sxs-lookup"><span data-stu-id="191b7-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="191b7-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="191b7-162">Request</span></span>
<span data-ttu-id="191b7-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="191b7-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="191b7-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="191b7-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="191b7-165">C#</span><span class="sxs-lookup"><span data-stu-id="191b7-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="191b7-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="191b7-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="191b7-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="191b7-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="191b7-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="191b7-168">Response</span></span>
<span data-ttu-id="191b7-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="191b7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
