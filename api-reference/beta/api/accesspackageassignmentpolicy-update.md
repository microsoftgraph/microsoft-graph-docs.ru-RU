---
title: Обновление accessPackageAssignmentPolicy
description: Обновление свойств объекта accessPackageAssignmentPolicy.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5a32ed205a10035e234a540f0048867e3bee4fa4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719234"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="452f3-103">Обновление accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="452f3-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="452f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="452f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="452f3-105">Обнови [существующий объект accessPackageAssignmentPolicy,](../resources/accesspackageassignmentpolicy.md) чтобы изменить одно или несколько его свойств, например имя или описание отображения.</span><span class="sxs-lookup"><span data-stu-id="452f3-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="452f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="452f3-106">Permissions</span></span>
<span data-ttu-id="452f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="452f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="452f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="452f3-109">Permission type</span></span>|<span data-ttu-id="452f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="452f3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="452f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="452f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="452f3-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="452f3-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="452f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="452f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="452f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="452f3-114">Not supported.</span></span> |
|<span data-ttu-id="452f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="452f3-115">Application</span></span>                            | <span data-ttu-id="452f3-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="452f3-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="452f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="452f3-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="452f3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="452f3-118">Request headers</span></span>
|<span data-ttu-id="452f3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="452f3-119">Name</span></span>|<span data-ttu-id="452f3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="452f3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="452f3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="452f3-121">Authorization</span></span>|<span data-ttu-id="452f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="452f3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="452f3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="452f3-124">Content-Type</span></span>|<span data-ttu-id="452f3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="452f3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="452f3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="452f3-127">Request body</span></span>
<span data-ttu-id="452f3-128">В теле запроса поставляем представление JSON объекта [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="452f3-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="452f3-129">В следующей таблице показаны свойства, необходимые при обновлении [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="452f3-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="452f3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="452f3-130">Property</span></span>|<span data-ttu-id="452f3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="452f3-131">Type</span></span>|<span data-ttu-id="452f3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="452f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="452f3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="452f3-133">displayName</span></span>|<span data-ttu-id="452f3-134">String</span><span class="sxs-lookup"><span data-stu-id="452f3-134">String</span></span>|<span data-ttu-id="452f3-135">Отображает имя политики.</span><span class="sxs-lookup"><span data-stu-id="452f3-135">The display name of the policy.</span></span>|
|<span data-ttu-id="452f3-136">description</span><span class="sxs-lookup"><span data-stu-id="452f3-136">description</span></span>|<span data-ttu-id="452f3-137">String</span><span class="sxs-lookup"><span data-stu-id="452f3-137">String</span></span>|<span data-ttu-id="452f3-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="452f3-138">The description of the policy.</span></span>|
|<span data-ttu-id="452f3-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="452f3-139">canExtend</span></span>|<span data-ttu-id="452f3-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="452f3-140">Boolean</span></span>|<span data-ttu-id="452f3-141">Указывает, может ли пользователь продлить срок назначения пакета доступа после утверждения.</span><span class="sxs-lookup"><span data-stu-id="452f3-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="452f3-142">durationInDays</span><span class="sxs-lookup"><span data-stu-id="452f3-142">durationInDays</span></span>|<span data-ttu-id="452f3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="452f3-143">Int32</span></span>|<span data-ttu-id="452f3-144">Количество дней, в течение которых назначения из этой политики будут выполняться до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="452f3-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="452f3-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="452f3-145">expirationDateTime</span></span>|<span data-ttu-id="452f3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="452f3-146">DateTimeOffset</span></span>|<span data-ttu-id="452f3-147">Срок действия для назначений, созданных в этой политике.</span><span class="sxs-lookup"><span data-stu-id="452f3-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="452f3-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="452f3-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="452f3-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="452f3-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="452f3-150">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="452f3-150">requestorSettings</span></span>|[<span data-ttu-id="452f3-151">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="452f3-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="452f3-152">Кто может запросить этот пакет доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="452f3-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="452f3-153">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="452f3-153">requestApprovalSettings</span></span>|[<span data-ttu-id="452f3-154">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="452f3-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="452f3-155">Кто должен утверждать запросы на пакет доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="452f3-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="452f3-156">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="452f3-156">accessReviewSettings</span></span>|[<span data-ttu-id="452f3-157">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="452f3-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="452f3-158">Кто должен и как часто выполнять назначения пакету доступа из этой политики.</span><span class="sxs-lookup"><span data-stu-id="452f3-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="452f3-159">Это свойство является null, если отзывы не требуются.</span><span class="sxs-lookup"><span data-stu-id="452f3-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="452f3-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="452f3-160">Response</span></span>
<span data-ttu-id="452f3-161">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="452f3-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="452f3-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="452f3-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="452f3-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="452f3-163">Request</span></span>
<span data-ttu-id="452f3-164">В этом обновлении политики был удален один из вариантов нескольких вариантов выбора.</span><span class="sxs-lookup"><span data-stu-id="452f3-164">In this policy update, one of the options for the multiple choice question was removed.</span></span> <span data-ttu-id="452f3-165">Будущие запросчики больше не будут иметь удаленную опцию, доступную для них.</span><span class="sxs-lookup"><span data-stu-id="452f3-165">Future requestors will no longer have the removed option available to them.</span></span>

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
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true,
        "allowedRequestors": []
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [{
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ]
            }
        ]
    },
    "accessReviewSettings": {
        "isEnabled": false
    },
    "questions": [{
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```


# <a name="java"></a>[<span data-ttu-id="452f3-166">Java</span><span class="sxs-lookup"><span data-stu-id="452f3-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="452f3-167">C#</span><span class="sxs-lookup"><span data-stu-id="452f3-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="452f3-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="452f3-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="452f3-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="452f3-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="452f3-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="452f3-170">Response</span></span>
<span data-ttu-id="452f3-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="452f3-171">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "questions": [{
        "id" : "BD3F6B95-458D-4BC8-A9A6-8D4B29F64F3D",
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "id" : "F652C13C-A660-4E4C-A1E0-CE9FEC6EE57A",
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
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


