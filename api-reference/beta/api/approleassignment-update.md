---
title: Обновление объекта AppRoleAssignment
description: Обновление свойств объекта аппролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: a3aeea70142c81c7ce368d0c9e688c87677eb210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322623"
---
# <a name="update-approleassignment"></a><span data-ttu-id="2e31b-103">Обновление объекта AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2e31b-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e31b-104">Обновление свойств объекта аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="2e31b-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e31b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e31b-105">Permissions</span></span>
<span data-ttu-id="2e31b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e31b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e31b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e31b-108">Permission type</span></span>      | <span data-ttu-id="2e31b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e31b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e31b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e31b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e31b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e31b-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="2e31b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e31b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e31b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e31b-113">Not supported.</span></span>    |
|<span data-ttu-id="2e31b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e31b-114">Application</span></span> | <span data-ttu-id="2e31b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e31b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e31b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e31b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e31b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e31b-117">Request headers</span></span>
| <span data-ttu-id="2e31b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2e31b-118">Name</span></span>       | <span data-ttu-id="2e31b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2e31b-119">Type</span></span> | <span data-ttu-id="2e31b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e31b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e31b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e31b-121">Authorization</span></span>  | <span data-ttu-id="2e31b-122">string</span><span class="sxs-lookup"><span data-stu-id="2e31b-122">string</span></span>  | <span data-ttu-id="2e31b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e31b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e31b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e31b-125">Request body</span></span>
<span data-ttu-id="2e31b-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2e31b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e31b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e31b-129">Property</span></span>     | <span data-ttu-id="2e31b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2e31b-130">Type</span></span>   |<span data-ttu-id="2e31b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2e31b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e31b-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="2e31b-132">creationTimestamp</span></span>|<span data-ttu-id="2e31b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e31b-133">DateTimeOffset</span></span>|<span data-ttu-id="2e31b-134">Время создания гранта.</span><span class="sxs-lookup"><span data-stu-id="2e31b-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="2e31b-135">id</span><span class="sxs-lookup"><span data-stu-id="2e31b-135">id</span></span>|<span data-ttu-id="2e31b-136">GUID</span><span class="sxs-lookup"><span data-stu-id="2e31b-136">Guid</span></span>|<span data-ttu-id="2e31b-137">Идентификатор роли, назначенный субъекту.</span><span class="sxs-lookup"><span data-stu-id="2e31b-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="2e31b-138">Эта роль должна быть объявлена в целевом приложении-ресурсе **resourceId** в свойстве **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="2e31b-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="2e31b-139">Если в ресурсе не объявлены разрешения, необходимо указать идентификатор по умолчанию (нулевой GUID).</span><span class="sxs-lookup"><span data-stu-id="2e31b-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="2e31b-140">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="2e31b-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="2e31b-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e31b-141">principalDisplayName</span></span>|<span data-ttu-id="2e31b-142">String</span><span class="sxs-lookup"><span data-stu-id="2e31b-142">String</span></span>|<span data-ttu-id="2e31b-143">Отображаемое имя субъекта, которому был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="2e31b-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="2e31b-144">principalId</span><span class="sxs-lookup"><span data-stu-id="2e31b-144">principalId</span></span>|<span data-ttu-id="2e31b-145">GUID</span><span class="sxs-lookup"><span data-stu-id="2e31b-145">Guid</span></span>|<span data-ttu-id="2e31b-146">Уникальный идентификатор (**ObjectID**) субъекта, которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="2e31b-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="2e31b-147">**Примечания**: обязательные.</span><span class="sxs-lookup"><span data-stu-id="2e31b-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="2e31b-148">principalType</span><span class="sxs-lookup"><span data-stu-id="2e31b-148">principalType</span></span>|<span data-ttu-id="2e31b-149">String</span><span class="sxs-lookup"><span data-stu-id="2e31b-149">String</span></span>|<span data-ttu-id="2e31b-150">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="2e31b-150">The type of principal.</span></span>  <span data-ttu-id="2e31b-151">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="2e31b-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="2e31b-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e31b-152">resourceDisplayName</span></span>|<span data-ttu-id="2e31b-153">String</span><span class="sxs-lookup"><span data-stu-id="2e31b-153">String</span></span>|<span data-ttu-id="2e31b-154">Отображаемое имя ресурса, для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="2e31b-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="2e31b-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e31b-155">resourceId</span></span>|<span data-ttu-id="2e31b-156">GUID</span><span class="sxs-lookup"><span data-stu-id="2e31b-156">Guid</span></span>|<span data-ttu-id="2e31b-157">Уникальный идентификатор (**ObjectID**) для целевого ресурса (субъекта-службы), для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="2e31b-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="2e31b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e31b-158">Response</span></span>

<span data-ttu-id="2e31b-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e31b-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e31b-160">Пример</span><span class="sxs-lookup"><span data-stu-id="2e31b-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e31b-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e31b-161">Request</span></span>
<span data-ttu-id="2e31b-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e31b-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2e31b-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e31b-163">Response</span></span>
<span data-ttu-id="2e31b-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e31b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
