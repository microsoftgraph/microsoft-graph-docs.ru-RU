---
title: Обновление approleassignment
description: Обновление свойства объекта approleassignment.
localization_priority: Normal
ms.openlocfilehash: 3d0f95e5413354a28e7b9b26e9b440f147c45931
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809634"
---
# <a name="update-approleassignment"></a><span data-ttu-id="2bce3-103">Обновление approleassignment</span><span class="sxs-lookup"><span data-stu-id="2bce3-103">Update approleassignment</span></span>

> <span data-ttu-id="2bce3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2bce3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bce3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bce3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bce3-106">Обновление свойства объекта approleassignment.</span><span class="sxs-lookup"><span data-stu-id="2bce3-106">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2bce3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bce3-107">Permissions</span></span>
<span data-ttu-id="2bce3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bce3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bce3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bce3-110">Permission type</span></span>      | <span data-ttu-id="2bce3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bce3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bce3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bce3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2bce3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bce3-113">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="2bce3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bce3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bce3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bce3-115">Not supported.</span></span>    |
|<span data-ttu-id="2bce3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bce3-116">Application</span></span> | <span data-ttu-id="2bce3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bce3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bce3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bce3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2bce3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bce3-119">Request headers</span></span>
| <span data-ttu-id="2bce3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2bce3-120">Name</span></span>       | <span data-ttu-id="2bce3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2bce3-121">Type</span></span> | <span data-ttu-id="2bce3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2bce3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2bce3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bce3-123">Authorization</span></span>  | <span data-ttu-id="2bce3-124">string</span><span class="sxs-lookup"><span data-stu-id="2bce3-124">string</span></span>  | <span data-ttu-id="2bce3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bce3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bce3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bce3-127">Request body</span></span>
<span data-ttu-id="2bce3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2bce3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2bce3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bce3-131">Property</span></span>     | <span data-ttu-id="2bce3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2bce3-132">Type</span></span>   |<span data-ttu-id="2bce3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2bce3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bce3-134">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="2bce3-134">creationTimestamp</span></span>|<span data-ttu-id="2bce3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bce3-135">DateTimeOffset</span></span>|<span data-ttu-id="2bce3-136">Время создания разрешений.</span><span class="sxs-lookup"><span data-stu-id="2bce3-136">The time when the grant was created.</span></span>|
|<span data-ttu-id="2bce3-137">id</span><span class="sxs-lookup"><span data-stu-id="2bce3-137">id</span></span>|<span data-ttu-id="2bce3-138">Guid</span><span class="sxs-lookup"><span data-stu-id="2bce3-138">Guid</span></span>|<span data-ttu-id="2bce3-139">Идентификатор роли, которая была назначена субъекта.</span><span class="sxs-lookup"><span data-stu-id="2bce3-139">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="2bce3-140">Эта роль должны быть объявлены с приложения ресурсов конечного **Ид_ресурса** в своем свойстве **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="2bce3-140">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="2bce3-141">Где ресурса не объявляет никаких разрешений, должен быть указан идентификатор по умолчанию (нулевое значение GUID).</span><span class="sxs-lookup"><span data-stu-id="2bce3-141">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="2bce3-142">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="2bce3-142">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="2bce3-143">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="2bce3-143">principalDisplayName</span></span>|<span data-ttu-id="2bce3-144">Строка</span><span class="sxs-lookup"><span data-stu-id="2bce3-144">String</span></span>|<span data-ttu-id="2bce3-145">Отображаемое имя субъекта, который был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="2bce3-145">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="2bce3-146">principalId</span><span class="sxs-lookup"><span data-stu-id="2bce3-146">principalId</span></span>|<span data-ttu-id="2bce3-147">Guid</span><span class="sxs-lookup"><span data-stu-id="2bce3-147">Guid</span></span>|<span data-ttu-id="2bce3-148">Уникальный идентификатор (**objectId**) для участника, которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="2bce3-148">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="2bce3-149">**Примечания**: обязательные.</span><span class="sxs-lookup"><span data-stu-id="2bce3-149">**Notes**: required.</span></span>            |
|<span data-ttu-id="2bce3-150">principalType</span><span class="sxs-lookup"><span data-stu-id="2bce3-150">principalType</span></span>|<span data-ttu-id="2bce3-151">Строка</span><span class="sxs-lookup"><span data-stu-id="2bce3-151">String</span></span>|<span data-ttu-id="2bce3-152">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="2bce3-152">The type of principal.</span></span>  <span data-ttu-id="2bce3-153">Это может быть «User», «Группы» или «ServicePrincipal».</span><span class="sxs-lookup"><span data-stu-id="2bce3-153">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="2bce3-154">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2bce3-154">resourceDisplayName</span></span>|<span data-ttu-id="2bce3-155">Строка</span><span class="sxs-lookup"><span data-stu-id="2bce3-155">String</span></span>|<span data-ttu-id="2bce3-156">Отображаемое имя ресурса, к которому назначения.</span><span class="sxs-lookup"><span data-stu-id="2bce3-156">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="2bce3-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="2bce3-157">resourceId</span></span>|<span data-ttu-id="2bce3-158">Guid</span><span class="sxs-lookup"><span data-stu-id="2bce3-158">Guid</span></span>|<span data-ttu-id="2bce3-159">Уникальный идентификатор (**objectId**) целевой ресурс, для которого было выполнено назначение (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="2bce3-159">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="2bce3-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bce3-160">Response</span></span>

<span data-ttu-id="2bce3-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [appRoleAssignment](../resources/approleassignment.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2bce3-161">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bce3-162">Пример</span><span class="sxs-lookup"><span data-stu-id="2bce3-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bce3-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bce3-163">Request</span></span>
<span data-ttu-id="2bce3-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bce3-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2bce3-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bce3-165">Response</span></span>
<span data-ttu-id="2bce3-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2bce3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
