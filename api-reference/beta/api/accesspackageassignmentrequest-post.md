---
title: Создание Акцесспаккажеассигнментрекуест
description: Создание нового Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90530cb12ece487c440fee2f1283dec787cda709
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936047"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="db4a4-103">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="db4a4-103">Create accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db4a4-104">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)создайте новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="db4a4-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db4a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db4a4-105">Permissions</span></span>

<span data-ttu-id="db4a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db4a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db4a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db4a4-108">Permission type</span></span>                        | <span data-ttu-id="db4a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db4a4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db4a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db4a4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="db4a4-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="db4a4-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="db4a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db4a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db4a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db4a4-113">Not supported.</span></span> |
| <span data-ttu-id="db4a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db4a4-114">Application</span></span>                            | <span data-ttu-id="db4a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db4a4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db4a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db4a4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="db4a4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db4a4-117">Request headers</span></span>

| <span data-ttu-id="db4a4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="db4a4-118">Name</span></span>          | <span data-ttu-id="db4a4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="db4a4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db4a4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="db4a4-120">Authorization</span></span> | <span data-ttu-id="db4a4-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="db4a4-121">Bearer \{token\}.</span></span> <span data-ttu-id="db4a4-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="db4a4-122">Required.</span></span> |
| <span data-ttu-id="db4a4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db4a4-123">Content-Type</span></span>  | <span data-ttu-id="db4a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="db4a4-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db4a4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db4a4-125">Request body</span></span>

<span data-ttu-id="db4a4-126">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db4a4-126">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db4a4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="db4a4-127">Response</span></span>

<span data-ttu-id="db4a4-128">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db4a4-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db4a4-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="db4a4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db4a4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="db4a4-130">Request</span></span>

<span data-ttu-id="db4a4-131">Ниже приведен пример запроса для прямого назначения.</span><span class="sxs-lookup"><span data-stu-id="db4a4-131">The following is an example of the request for a direct assignment.</span></span>  <span data-ttu-id="db4a4-132">Значение параметра `targetID` — это идентификатор объекта, которому назначен пользователь, значение которого `accessPackageId` является необходимым пакетом доступа, а значение `assignmentPolicyId` — это прямая политика назначения в этом пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="db4a4-132">The value of the `targetID` is the object ID of a user being assigned, the value of the `accessPackageId` is the desired access package, and the value of `assignmentPolicyId` is a direct assignment policy in that access package.</span></span>
 
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

### <a name="response"></a><span data-ttu-id="db4a4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="db4a4-133">Response</span></span>

<span data-ttu-id="db4a4-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db4a4-134">The following is an example of the response.</span></span>

> <span data-ttu-id="db4a4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db4a4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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