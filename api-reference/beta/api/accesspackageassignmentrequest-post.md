---
title: Создание Акцесспаккажеассигнментрекуест
description: Создание нового Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 128c4c84879ec11c6ac0b54991247b84125285f2
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108408"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="ba499-103">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ba499-103">Create accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba499-104">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)создайте новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ba499-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="ba499-105">Эта операция используется для назначения пользователя в пакет Access или для удаления назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="ba499-105">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba499-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba499-106">Permissions</span></span>

<span data-ttu-id="ba499-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba499-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba499-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba499-109">Permission type</span></span>                        | <span data-ttu-id="ba499-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba499-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba499-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba499-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba499-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba499-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ba499-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba499-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba499-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba499-114">Not supported.</span></span> |
| <span data-ttu-id="ba499-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba499-115">Application</span></span>                            | <span data-ttu-id="ba499-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba499-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba499-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba499-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="ba499-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba499-118">Request headers</span></span>

| <span data-ttu-id="ba499-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba499-119">Name</span></span>          | <span data-ttu-id="ba499-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba499-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ba499-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba499-121">Authorization</span></span> | <span data-ttu-id="ba499-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="ba499-122">Bearer \{token\}.</span></span> <span data-ttu-id="ba499-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ba499-123">Required.</span></span> |
| <span data-ttu-id="ba499-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba499-124">Content-Type</span></span>  | <span data-ttu-id="ba499-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba499-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba499-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba499-127">Request body</span></span>

<span data-ttu-id="ba499-128">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba499-128">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="ba499-129">Чтобы `AdminAdd`создать назначение для пользователя, используется значение свойства **requestType** , а свойство **акцесспаккажеассигнмент** `targetId` содержит назначенного пользователя, свойство **ассигнментполициид** , идентифицирующее [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md), и свойство **акцесспаккажеид** , определяющее [accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="ba499-129">To create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="ba499-130">Чтобы удалить назначение, значение свойства **requestType** — `AdminRemove`, и свойство **акцесспаккажеассигнмент** содержит свойство **ID** , идентифицирующее удаляемое [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ba499-130">To remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

## <a name="response"></a><span data-ttu-id="ba499-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba499-131">Response</span></span>

<span data-ttu-id="ba499-132">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba499-132">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba499-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba499-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba499-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba499-134">Request</span></span>

<span data-ttu-id="ba499-135">Ниже приведен пример запроса для прямого назначения.</span><span class="sxs-lookup"><span data-stu-id="ba499-135">The following is an example of the request for a direct assignment.</span></span>  <span data-ttu-id="ba499-136">Значение **targetID** — это идентификатор объекта, которому назначен пользователь, значение **акцесспаккажеид** — это необходимый пакет доступа, а значение **ассигнментполициид** — это прямая политика назначения в этом пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="ba499-136">The value of the **targetID** is the object ID of a user being assigned, the value of the **accessPackageId** is the desired access package, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="ba499-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba499-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba499-138">C#</span><span class="sxs-lookup"><span data-stu-id="ba499-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba499-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba499-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba499-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba499-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba499-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba499-141">Response</span></span>

<span data-ttu-id="ba499-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba499-142">The following is an example of the response.</span></span>

> <span data-ttu-id="ba499-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba499-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
