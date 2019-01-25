---
title: Обновление approleassignment
description: Обновление свойства объекта approleassignment.
localization_priority: Normal
ms.openlocfilehash: 54c256e3b94a5bb2d62c2ffe31ecf777d472b93c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527922"
---
# <a name="update-approleassignment"></a><span data-ttu-id="a7dc1-103">Обновление approleassignment</span><span class="sxs-lookup"><span data-stu-id="a7dc1-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7dc1-104">Обновление свойства объекта approleassignment.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7dc1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7dc1-105">Permissions</span></span>
<span data-ttu-id="a7dc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7dc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7dc1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7dc1-108">Permission type</span></span>      | <span data-ttu-id="a7dc1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7dc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7dc1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7dc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7dc1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7dc1-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="a7dc1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7dc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7dc1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-113">Not supported.</span></span>    |
|<span data-ttu-id="a7dc1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7dc1-114">Application</span></span> | <span data-ttu-id="a7dc1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7dc1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7dc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a7dc1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7dc1-117">Request headers</span></span>
| <span data-ttu-id="a7dc1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a7dc1-118">Name</span></span>       | <span data-ttu-id="a7dc1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a7dc1-119">Type</span></span> | <span data-ttu-id="a7dc1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dc1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7dc1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7dc1-121">Authorization</span></span>  | <span data-ttu-id="a7dc1-122">string</span><span class="sxs-lookup"><span data-stu-id="a7dc1-122">string</span></span>  | <span data-ttu-id="a7dc1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7dc1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7dc1-125">Request body</span></span>
<span data-ttu-id="a7dc1-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7dc1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7dc1-129">Property</span></span>     | <span data-ttu-id="a7dc1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a7dc1-130">Type</span></span>   |<span data-ttu-id="a7dc1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dc1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7dc1-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="a7dc1-132">creationTimestamp</span></span>|<span data-ttu-id="a7dc1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7dc1-133">DateTimeOffset</span></span>|<span data-ttu-id="a7dc1-134">Время создания разрешений.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="a7dc1-135">id</span><span class="sxs-lookup"><span data-stu-id="a7dc1-135">id</span></span>|<span data-ttu-id="a7dc1-136">Guid</span><span class="sxs-lookup"><span data-stu-id="a7dc1-136">Guid</span></span>|<span data-ttu-id="a7dc1-137">Идентификатор роли, которая была назначена субъекта.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="a7dc1-138">Эта роль должны быть объявлены с приложения ресурсов конечного **Ид_ресурса** в своем свойстве **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="a7dc1-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="a7dc1-139">Где ресурса не объявляет никаких разрешений, должен быть указан идентификатор по умолчанию (нулевое значение GUID).</span><span class="sxs-lookup"><span data-stu-id="a7dc1-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="a7dc1-140">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="a7dc1-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7dc1-141">principalDisplayName</span></span>|<span data-ttu-id="a7dc1-142">String</span><span class="sxs-lookup"><span data-stu-id="a7dc1-142">String</span></span>|<span data-ttu-id="a7dc1-143">Отображаемое имя субъекта, который был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="a7dc1-144">principalId</span><span class="sxs-lookup"><span data-stu-id="a7dc1-144">principalId</span></span>|<span data-ttu-id="a7dc1-145">Guid</span><span class="sxs-lookup"><span data-stu-id="a7dc1-145">Guid</span></span>|<span data-ttu-id="a7dc1-146">Уникальный идентификатор (**objectId**) для участника, которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="a7dc1-147">**Примечания**: обязательные.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="a7dc1-148">principalType</span><span class="sxs-lookup"><span data-stu-id="a7dc1-148">principalType</span></span>|<span data-ttu-id="a7dc1-149">String</span><span class="sxs-lookup"><span data-stu-id="a7dc1-149">String</span></span>|<span data-ttu-id="a7dc1-150">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-150">The type of principal.</span></span>  <span data-ttu-id="a7dc1-151">Это может быть «User», «Группы» или «ServicePrincipal».</span><span class="sxs-lookup"><span data-stu-id="a7dc1-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="a7dc1-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7dc1-152">resourceDisplayName</span></span>|<span data-ttu-id="a7dc1-153">String</span><span class="sxs-lookup"><span data-stu-id="a7dc1-153">String</span></span>|<span data-ttu-id="a7dc1-154">Отображаемое имя ресурса, к которому назначения.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="a7dc1-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="a7dc1-155">resourceId</span></span>|<span data-ttu-id="a7dc1-156">Guid</span><span class="sxs-lookup"><span data-stu-id="a7dc1-156">Guid</span></span>|<span data-ttu-id="a7dc1-157">Уникальный идентификатор (**objectId**) целевой ресурс, для которого было выполнено назначение (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="a7dc1-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="a7dc1-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7dc1-158">Response</span></span>

<span data-ttu-id="a7dc1-159">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [appRoleAssignment](../resources/approleassignment.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7dc1-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a7dc1-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7dc1-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7dc1-161">Request</span></span>
<span data-ttu-id="a7dc1-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7dc1-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a7dc1-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7dc1-163">Response</span></span>
<span data-ttu-id="a7dc1-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a7dc1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
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
    "Error: /api-reference/beta/api/approleassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
