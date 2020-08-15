---
title: Обновление Акцесспаккажеассигнментполици
description: Обновление свойств объекта Акцесспаккажеассигнментполици.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a0d83dc1ca17baf5fd179efe225af8694b5ea6bb
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757485"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="b4038-103">Обновление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="b4038-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="b4038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4038-105">Обновление существующего объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="b4038-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4038-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4038-106">Permissions</span></span>
<span data-ttu-id="b4038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="b4038-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4038-109">Permission type</span></span>|<span data-ttu-id="b4038-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4038-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4038-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4038-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4038-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4038-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="b4038-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4038-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4038-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4038-114">Not supported.</span></span> |
|<span data-ttu-id="b4038-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4038-115">Application</span></span>                            | <span data-ttu-id="b4038-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4038-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4038-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4038-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="b4038-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4038-118">Request headers</span></span>
|<span data-ttu-id="b4038-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b4038-119">Name</span></span>|<span data-ttu-id="b4038-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b4038-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4038-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4038-121">Authorization</span></span>|<span data-ttu-id="b4038-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4038-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b4038-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4038-124">Content-Type</span></span>|<span data-ttu-id="b4038-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4038-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4038-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4038-127">Request body</span></span>
<span data-ttu-id="b4038-128">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4038-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="b4038-129">В следующей таблице приведены свойства, необходимые при обновлении [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b4038-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="b4038-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4038-130">Property</span></span>|<span data-ttu-id="b4038-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4038-131">Type</span></span>|<span data-ttu-id="b4038-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4038-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4038-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b4038-133">displayName</span></span>|<span data-ttu-id="b4038-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b4038-134">String</span></span>|<span data-ttu-id="b4038-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="b4038-135">The display name of the policy.</span></span>|
|<span data-ttu-id="b4038-136">description</span><span class="sxs-lookup"><span data-stu-id="b4038-136">description</span></span>|<span data-ttu-id="b4038-137">String</span><span class="sxs-lookup"><span data-stu-id="b4038-137">String</span></span>|<span data-ttu-id="b4038-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="b4038-138">The description of the policy.</span></span>|
|<span data-ttu-id="b4038-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="b4038-139">canExtend</span></span>|<span data-ttu-id="b4038-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4038-140">Boolean</span></span>|<span data-ttu-id="b4038-141">Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="b4038-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="b4038-142">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="b4038-142">durationInDays</span></span>|<span data-ttu-id="b4038-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b4038-143">Int32</span></span>|<span data-ttu-id="b4038-144">Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="b4038-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="b4038-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b4038-145">expirationDateTime</span></span>|<span data-ttu-id="b4038-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4038-146">DateTimeOffset</span></span>|<span data-ttu-id="b4038-147">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="b4038-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="b4038-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b4038-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b4038-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b4038-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b4038-150">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="b4038-150">requestorSettings</span></span>|[<span data-ttu-id="b4038-151">рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="b4038-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="b4038-152">Кто может запрашивать этот пакет Access из этой политики.</span><span class="sxs-lookup"><span data-stu-id="b4038-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="b4038-153">рекуестаппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="b4038-153">requestApprovalSettings</span></span>|[<span data-ttu-id="b4038-154">аппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="b4038-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="b4038-155">Кто должен утверждать запросы на пакет Access в этой политике.</span><span class="sxs-lookup"><span data-stu-id="b4038-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="b4038-156">акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b4038-156">accessReviewSettings</span></span>|[<span data-ttu-id="b4038-157">ассигнментревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b4038-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="b4038-158">Кто должен проверить и как часто назначений для пакета доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="b4038-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="b4038-159">Это свойство имеет значение null, если проверка не требуются.</span><span class="sxs-lookup"><span data-stu-id="b4038-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="b4038-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4038-160">Response</span></span>
<span data-ttu-id="b4038-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4038-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="b4038-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4038-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4038-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4038-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf
Content-Type: application/json
Content-length: 1000

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "requestorSettings" : {
    "scopeType": "AllExistingDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings" : {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  },
  "accessReviewSettings" : null
}
```


### <a name="response"></a><span data-ttu-id="b4038-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4038-164">Response</span></span>
<span data-ttu-id="b4038-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4038-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings" : null
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
