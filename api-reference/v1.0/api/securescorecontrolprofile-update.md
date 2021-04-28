---
title: Обновление объектов secureScoreControlProfile
description: Обновление редактируемого объекта secureScoreControlProfile в рамках любого интегрированного решения для изменения различных свойств, таких как назначеноTo или tenantNote.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d0ff440b19aaef21d3f33f6dff9e767d6b08a820
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038903"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="ad3e0-103">Обновление объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="ad3e0-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="ad3e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad3e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad3e0-105">Обновление редактируемого объекта **secureScoreControlProfile** в рамках любого интегрированного решения, чтобы изменить различные свойства, например **назначеноTo** или **tenantNote.**</span><span class="sxs-lookup"><span data-stu-id="ad3e0-105">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad3e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad3e0-106">Permissions</span></span>

<span data-ttu-id="ad3e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad3e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad3e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad3e0-109">Permission type</span></span>      | <span data-ttu-id="ad3e0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad3e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad3e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad3e0-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="ad3e0-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3e0-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="ad3e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad3e0-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ad3e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-114">Not supported.</span></span>  |
|<span data-ttu-id="ad3e0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad3e0-115">Application</span></span> | <span data-ttu-id="ad3e0-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3e0-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad3e0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad3e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ad3e0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad3e0-118">Request headers</span></span>

| <span data-ttu-id="ad3e0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ad3e0-119">Name</span></span>       | <span data-ttu-id="ad3e0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad3e0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ad3e0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad3e0-121">Authorization</span></span>  | <span data-ttu-id="ad3e0-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-122">Bearer {code}.</span></span> <span data-ttu-id="ad3e0-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-123">Required.</span></span>|
|<span data-ttu-id="ad3e0-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="ad3e0-124">Prefer</span></span> | <span data-ttu-id="ad3e0-125">return=representation.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad3e0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad3e0-126">Request body</span></span>

<span data-ttu-id="ad3e0-127">В теле запроса поставляем представление JSON значений для соответствующих полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ad3e0-128">Тело должно **содержать** свойство `vendorInformation` с допустимым и `provider` `vendor` полями.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-128">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="ad3e0-129">В следующей таблице перечислены поля, которые можно обновить для **secureScoreControlProfile.**</span><span class="sxs-lookup"><span data-stu-id="ad3e0-129">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="ad3e0-130">Значения для существующих свойств, не включенных в тело запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-130">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="ad3e0-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ad3e0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad3e0-132">Property</span></span>   | <span data-ttu-id="ad3e0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ad3e0-133">Type</span></span> |<span data-ttu-id="ad3e0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ad3e0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad3e0-135">assignedTo</span><span class="sxs-lookup"><span data-stu-id="ad3e0-135">assignedTo</span></span>|<span data-ttu-id="ad3e0-136">String</span><span class="sxs-lookup"><span data-stu-id="ad3e0-136">String</span></span>|<span data-ttu-id="ad3e0-137">Имя аналитика, на который назначен контроль для выполнения, выполнения или устранения.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-137">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="ad3e0-138">comment</span><span class="sxs-lookup"><span data-stu-id="ad3e0-138">comment</span></span>|<span data-ttu-id="ad3e0-139">String</span><span class="sxs-lookup"><span data-stu-id="ad3e0-139">String</span></span>|<span data-ttu-id="ad3e0-140">Аналитик комментирует управление (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="ad3e0-140">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="ad3e0-141">state</span><span class="sxs-lookup"><span data-stu-id="ad3e0-141">state</span></span>| <span data-ttu-id="ad3e0-142">String</span><span class="sxs-lookup"><span data-stu-id="ad3e0-142">String</span></span>|<span data-ttu-id="ad3e0-143">Параметр управления, управляемый аналитиком.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-143">Analyst driven setting on the control.</span></span> <span data-ttu-id="ad3e0-144">Возможные значения: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-144">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="ad3e0-145">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="ad3e0-145">vendorInformation</span></span> | [<span data-ttu-id="ad3e0-146">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="ad3e0-146">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="ad3e0-147">Сложный тип, содержащий сведения о поставщике продуктов и служб безопасности, поставщике и подпрограмме (например, поставщик=Microsoft; provider=SecureScore;).</span><span class="sxs-lookup"><span data-stu-id="ad3e0-147">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="ad3e0-148">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="ad3e0-148">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="ad3e0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad3e0-149">Response</span></span>

<span data-ttu-id="ad3e0-150">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-150">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="ad3e0-151">Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный объект `200 OK` [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-151">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad3e0-152">Пример</span><span class="sxs-lookup"><span data-stu-id="ad3e0-152">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="ad3e0-153">Пример 1. Запрос без загона Prefer</span><span class="sxs-lookup"><span data-stu-id="ad3e0-153">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="ad3e0-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad3e0-154">Request</span></span>

<span data-ttu-id="ad3e0-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad3e0-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad3e0-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {

    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ad3e0-157">C#</span><span class="sxs-lookup"><span data-stu-id="ad3e0-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad3e0-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad3e0-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad3e0-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad3e0-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad3e0-160">Java</span><span class="sxs-lookup"><span data-stu-id="ad3e0-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad3e0-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad3e0-161">Response</span></span>

<span data-ttu-id="ad3e0-162">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-162">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="ad3e0-163">Пример 2. Запрос с помощью загона Prefer</span><span class="sxs-lookup"><span data-stu-id="ad3e0-163">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="ad3e0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad3e0-164">Request</span></span>

<span data-ttu-id="ad3e0-165">В следующем примере показан запрос, который включает заглавную `Prefer` головку запроса.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-165">The following example shows a request that includes the `Prefer` request header.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad3e0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad3e0-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ad3e0-167">C#</span><span class="sxs-lookup"><span data-stu-id="ad3e0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad3e0-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad3e0-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad3e0-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad3e0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad3e0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad3e0-170">Response</span></span>

<span data-ttu-id="ad3e0-171">Ниже приводится пример ответа, когда используется необязательный `Prefer: return=representation` заглавной запрос.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-171">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="ad3e0-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad3e0-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "NonOwnerAccess",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Review",
  "actionUrl": "https://outlook.office365.com/NonOwnerAccessReport.aspx",
  "controlCategory": "Data",
  "title": "Review mailbox access by non-owners bi-weekly", 
  "deprecated": false,
  "implementationCost": "Low",
  "lastModifiedDateTime": null,
  "maxScore": 5.0,
  "rank": 25,
  "remediation": "Once you have opened the search tool, specify a date range and select access by <b>All non-owners</b> or <b>External users</b>",
  "remediationImpact": "This change will have no effect on your users",
  "service": "EXO",
  "threats": [
    "Account Breach",
    "Data Exfiltration",
    "Malicious Insider"
  ],
  "tier": "Core",
  "userImpact": "Low",
  "complianceInformation": [
    {
      "certificationName": "FedRAMP_Moderate",
      "certificationControls": [
        {
          "name": "AC-6(9)",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": "",
      "comment": "control is reviewed",
      "state": "Reviewed",
      "updatedBy": "user1@contoso.com",
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

