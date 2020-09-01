---
title: Создание Акцесспаккажеассигнментрекуест
description: Создание нового Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1318455b3a9307527f47af523efd7e8ac2680a8b
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319402"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="d72fe-103">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d72fe-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="d72fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d72fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d72fe-105">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)создайте новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d72fe-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="d72fe-106">Эта операция используется для назначения пользователя в пакет Access или для удаления назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d72fe-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d72fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d72fe-107">Permissions</span></span>

<span data-ttu-id="d72fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d72fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d72fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d72fe-110">Permission type</span></span>                        | <span data-ttu-id="d72fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d72fe-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d72fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d72fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d72fe-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d72fe-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d72fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d72fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d72fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d72fe-115">Not supported.</span></span> |
| <span data-ttu-id="d72fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d72fe-116">Application</span></span>                            | <span data-ttu-id="d72fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d72fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d72fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d72fe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="d72fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d72fe-119">Request headers</span></span>

| <span data-ttu-id="d72fe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d72fe-120">Name</span></span>          | <span data-ttu-id="d72fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d72fe-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d72fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d72fe-122">Authorization</span></span> | <span data-ttu-id="d72fe-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="d72fe-123">Bearer \{token\}.</span></span> <span data-ttu-id="d72fe-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d72fe-124">Required.</span></span> |
| <span data-ttu-id="d72fe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d72fe-125">Content-Type</span></span>  | <span data-ttu-id="d72fe-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d72fe-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d72fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d72fe-128">Request body</span></span>

<span data-ttu-id="d72fe-129">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d72fe-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="d72fe-130">Чтобы администратор запрашивал создание назначения для пользователя, свойство **requestType** имеет значение `AdminAdd` , а свойство **акцесспаккажеассигнмент** содержит `targetId` назначенного пользователя, свойство **ассигнментполициид** , идентифицирующее [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md), и свойство **акцесспаккажеид** , определяющее [accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="d72fe-130">For an administrator to request to create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="d72fe-131">Чтобы администратор запрашивал удаление назначения, свойство **requestType** имеет значение `AdminRemove` , а свойство **акцесспаккажеассигнмент** содержит свойство **ID** , идентифицирующее удаляемое [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d72fe-131">For an administrator to request to remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

<span data-ttu-id="d72fe-132">Чтобы пользователь, не являющийся администратором, запрашивался для самостоятельного создания назначения, используется значение свойства **requestType** `UserAdd` , а свойство **акцесспаккажеассигнмент** содержит `targetId` идентификатор самих пользователей, свойство **ассигнментполициид** , идентифицирующее [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md), и свойство **акцесспаккажеид** , определяющее [accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="d72fe-132">For a non-administrator user to request to create an assignment for themselves, the value of the **requestType** property is `UserAdd`, and the **accessPackageAssignment** property contains the `targetId` with the ID of the users themselves, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>  <span data-ttu-id="d72fe-133">Пользователь, выполняющий запрос, должен уже существовать в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d72fe-133">The user making the request must already exist in the directory.</span></span>

## <a name="response"></a><span data-ttu-id="d72fe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d72fe-134">Response</span></span>

<span data-ttu-id="d72fe-135">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d72fe-135">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>  

<span data-ttu-id="d72fe-136">Если это `AdminAdd` запрос, затем [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) и, при необходимости, также создаются [акцесспаккажесубжект](../resources/accesspackagesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="d72fe-136">If this is an `AdminAdd` request, then subsequently an [accessPackageAssignment](../resources/accesspackageassignment.md) and, if needed, an [accessPackageSubject](../resources/accesspackagesubject.md) are also created.</span></span> <span data-ttu-id="d72fe-137">Вы можете указать их, используя параметры запроса при [выводе акцесспаккажеассигнментс](accesspackageassignment-list.md).</span><span class="sxs-lookup"><span data-stu-id="d72fe-137">You can locate those using the query parameters when [listing accessPackageAssignments](accesspackageassignment-list.md).</span></span>

## <a name="examples"></a><span data-ttu-id="d72fe-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="d72fe-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d72fe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d72fe-139">Request</span></span>

<span data-ttu-id="d72fe-140">Ниже приведен пример запроса для прямого назначения, в котором администратор запрашивает создание назначения для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d72fe-140">The following is an example of the request for a direct assignment, in which the administrator is requesting the creation of an assignment for the user.</span></span> <span data-ttu-id="d72fe-141">Так как [акцесспаккажесубжект](../resources/accesspackagesubject.md) может еще не существовать, значение **TARGETID** — это идентификатор объекта, которому назначен пользователь, значение **акцесспаккажеид** — это необходимый пакет доступа для этого пользователя, а значение **ассигнментполициид** — это прямая политика назначения в этом пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="d72fe-141">Because the [accessPackageSubject](../resources/accesspackagesubject.md) might not yet exist, the value of the **targetID** is the object ID of the user being assigned, the value of the **accessPackageId** is the desired access package for that user, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="d72fe-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72fe-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d72fe-143">C#</span><span class="sxs-lookup"><span data-stu-id="d72fe-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d72fe-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72fe-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d72fe-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72fe-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d72fe-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d72fe-146">Response</span></span>

<span data-ttu-id="d72fe-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d72fe-147">The following is an example of the response.</span></span>

> <span data-ttu-id="d72fe-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d72fe-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
