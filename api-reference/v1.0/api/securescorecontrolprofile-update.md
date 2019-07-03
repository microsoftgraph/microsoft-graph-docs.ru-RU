---
title: Обновление объектов secureScoreControlProfile
description: Обновление редактируемого объекта Секурескореконтролпрофиле в любом интегрированном решении для изменения различных свойств, таких как assignedTo или Тенантноте.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: 8cf86d312d9f866c24cfc0d6fc11ba523885d627
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448304"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="9056d-103">Обновление объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="9056d-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="9056d-104">Обновление редактируемого объекта **секурескореконтролпрофиле** в любом интегрированном решении для изменения различных свойств, таких как **assignedTo** или **тенантноте**.</span><span class="sxs-lookup"><span data-stu-id="9056d-104">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="9056d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9056d-105">Permissions</span></span>

<span data-ttu-id="9056d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9056d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9056d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9056d-108">Permission type</span></span>      | <span data-ttu-id="9056d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9056d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9056d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9056d-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="9056d-111">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="9056d-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="9056d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9056d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9056d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9056d-113">Not supported.</span></span>  |
|<span data-ttu-id="9056d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9056d-114">Application</span></span> | <span data-ttu-id="9056d-115">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="9056d-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9056d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9056d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9056d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9056d-117">Request headers</span></span>

| <span data-ttu-id="9056d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9056d-118">Name</span></span>       | <span data-ttu-id="9056d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9056d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9056d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9056d-120">Authorization</span></span>  | <span data-ttu-id="9056d-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="9056d-121">Bearer {code}.</span></span> <span data-ttu-id="9056d-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9056d-122">Required.</span></span>|
|<span data-ttu-id="9056d-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="9056d-123">Prefer</span></span> | <span data-ttu-id="9056d-124">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="9056d-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9056d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9056d-125">Request body</span></span>

<span data-ttu-id="9056d-126">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9056d-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9056d-127">Текст **должен** содержать `vendorInformation` свойство Valid `provider` и `vendor` Fields.</span><span class="sxs-lookup"><span data-stu-id="9056d-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="9056d-128">В следующей таблице перечислены поля, которые можно обновить для **секурескореконтролпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="9056d-128">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="9056d-129">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="9056d-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="9056d-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9056d-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9056d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9056d-131">Property</span></span>   | <span data-ttu-id="9056d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9056d-132">Type</span></span> |<span data-ttu-id="9056d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9056d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9056d-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="9056d-134">assignedTo</span></span>|<span data-ttu-id="9056d-135">String</span><span class="sxs-lookup"><span data-stu-id="9056d-135">String</span></span>|<span data-ttu-id="9056d-136">Имя аналитики, которой назначен элемент управления для рассмотрения, внедрения или исправления.</span><span class="sxs-lookup"><span data-stu-id="9056d-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="9056d-137">comment</span><span class="sxs-lookup"><span data-stu-id="9056d-137">comment</span></span>|<span data-ttu-id="9056d-138">String</span><span class="sxs-lookup"><span data-stu-id="9056d-138">String</span></span>|<span data-ttu-id="9056d-139">Комментарии аналитика в элементе управления (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="9056d-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="9056d-140">state</span><span class="sxs-lookup"><span data-stu-id="9056d-140">state</span></span>| <span data-ttu-id="9056d-141">String</span><span class="sxs-lookup"><span data-stu-id="9056d-141">String</span></span>|<span data-ttu-id="9056d-142">Управляемый аналитикой параметр для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="9056d-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="9056d-143">Возможные значения: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span><span class="sxs-lookup"><span data-stu-id="9056d-143">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="9056d-144">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="9056d-144">vendorInformation</span></span> | [<span data-ttu-id="9056d-145">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="9056d-145">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="9056d-146">Сложный тип, содержащий сведения о продукте, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре;).</span><span class="sxs-lookup"><span data-stu-id="9056d-146">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="9056d-147">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="9056d-147">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="9056d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9056d-148">Response</span></span>

<span data-ttu-id="9056d-149">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9056d-149">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="9056d-150">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [секурескореконтролпрофилес](../resources/securescorecontrolprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9056d-150">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9056d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="9056d-151">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="9056d-152">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="9056d-152">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="9056d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="9056d-153">Request</span></span>

<span data-ttu-id="9056d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9056d-154">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9056d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="9056d-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9056d-156">C#</span><span class="sxs-lookup"><span data-stu-id="9056d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9056d-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="9056d-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9056d-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9056d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9056d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="9056d-159">Response</span></span>

<span data-ttu-id="9056d-160">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="9056d-160">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="9056d-161">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="9056d-161">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="9056d-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="9056d-162">Request</span></span>

<span data-ttu-id="9056d-163">В приведенном ниже примере показан запрос, включающий заголовок `Prefer` запроса.</span><span class="sxs-lookup"><span data-stu-id="9056d-163">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
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

#### <a name="response"></a><span data-ttu-id="9056d-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="9056d-164">Response</span></span>

<span data-ttu-id="9056d-165">Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.</span><span class="sxs-lookup"><span data-stu-id="9056d-165">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="9056d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9056d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
