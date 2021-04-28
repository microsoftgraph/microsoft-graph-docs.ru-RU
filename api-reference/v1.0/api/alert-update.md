---
title: Обновление оповещения
description: Обновление свойства редактируемого **оповещения** в любом интегрированном решении, чтобы синхронизировать состояние оповещений и назначения между решениями. Этот метод обновляет любое решение, которое имеет запись ссылаемого ID оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 863496528fdcd60d501fbc9c38e8fbb6ed1884dc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054660"
---
# <a name="update-alert"></a><span data-ttu-id="71b7e-104">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="71b7e-104">Update alert</span></span>

<span data-ttu-id="71b7e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b7e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71b7e-106">Обновление свойства редактируемого **оповещения** в любом интегрированном решении, чтобы синхронизировать состояние оповещений и назначения между решениями.</span><span class="sxs-lookup"><span data-stu-id="71b7e-106">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="71b7e-107">Этот метод обновляет любое решение, которое имеет запись ссылаемого ID оповещения.</span><span class="sxs-lookup"><span data-stu-id="71b7e-107">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="71b7e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71b7e-108">Permissions</span></span>

<span data-ttu-id="71b7e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71b7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71b7e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71b7e-111">Permission type</span></span>                        | <span data-ttu-id="71b7e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71b7e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="71b7e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71b7e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="71b7e-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71b7e-114">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="71b7e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71b7e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b7e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b7e-116">Not supported.</span></span>                      |
| <span data-ttu-id="71b7e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71b7e-117">Application</span></span>                            | <span data-ttu-id="71b7e-118">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71b7e-118">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="71b7e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71b7e-119">HTTP request</span></span>

> <span data-ttu-id="71b7e-120">**Примечание:** Необходимо включить **в** качестве параметра и поставщика ID оповещений, содержащего и `provider` с помощью этого `vendor` метода.</span><span class="sxs-lookup"><span data-stu-id="71b7e-120">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="71b7e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71b7e-121">Request headers</span></span>

| <span data-ttu-id="71b7e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="71b7e-122">Name</span></span>          | <span data-ttu-id="71b7e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="71b7e-123">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="71b7e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71b7e-124">Authorization</span></span> | <span data-ttu-id="71b7e-125">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="71b7e-125">Bearer {code}.</span></span> <span data-ttu-id="71b7e-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71b7e-126">Required.</span></span> |
| <span data-ttu-id="71b7e-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="71b7e-127">Prefer</span></span>        | <span data-ttu-id="71b7e-128">return=representation.</span><span class="sxs-lookup"><span data-stu-id="71b7e-128">return=representation.</span></span> <span data-ttu-id="71b7e-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="71b7e-129">Optional.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="71b7e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71b7e-130">Request body</span></span>

<span data-ttu-id="71b7e-131">В теле запроса поставляем представление JSON значений для соответствующих полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="71b7e-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="71b7e-132">Тело должно **содержать** свойство **vendorInformation** с допустимым и `provider` `vendor` полями.</span><span class="sxs-lookup"><span data-stu-id="71b7e-132">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="71b7e-133">В следующей таблице перечислены поля, которые можно обновить для оповещения.</span><span class="sxs-lookup"><span data-stu-id="71b7e-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="71b7e-134">Значения для существующих свойств, не включенных в тело запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="71b7e-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="71b7e-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="71b7e-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71b7e-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="71b7e-136">Property</span></span>          | <span data-ttu-id="71b7e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="71b7e-137">Type</span></span>                                                                   | <span data-ttu-id="71b7e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="71b7e-138">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="71b7e-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="71b7e-139">assignedTo</span></span>        | <span data-ttu-id="71b7e-140">String</span><span class="sxs-lookup"><span data-stu-id="71b7e-140">String</span></span>                                                                 | <span data-ttu-id="71b7e-141">Имя аналитика, на которое назначено оповещение для проверки, исследования или восстановления.</span><span class="sxs-lookup"><span data-stu-id="71b7e-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="71b7e-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="71b7e-142">closedDateTime</span></span>    | <span data-ttu-id="71b7e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71b7e-143">DateTimeOffset</span></span>                                                         | <span data-ttu-id="71b7e-144">Время закрытия оповещения.</span><span class="sxs-lookup"><span data-stu-id="71b7e-144">Time at which the alert was closed.</span></span> <span data-ttu-id="71b7e-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="71b7e-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71b7e-146">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="71b7e-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="71b7e-147">comments</span><span class="sxs-lookup"><span data-stu-id="71b7e-147">comments</span></span>          | <span data-ttu-id="71b7e-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71b7e-148">String collection</span></span>                                                      | <span data-ttu-id="71b7e-149">Аналитик комментирует оповещение (для управления оповещениями клиентов).</span><span class="sxs-lookup"><span data-stu-id="71b7e-149">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="71b7e-150">Этот метод может обновлять поле комментариев только с помощью следующих значений: `Closed in IPC` , `Closed in MCAS` .</span><span class="sxs-lookup"><span data-stu-id="71b7e-150">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span> |
| <span data-ttu-id="71b7e-151">feedback</span><span class="sxs-lookup"><span data-stu-id="71b7e-151">feedback</span></span>          | <span data-ttu-id="71b7e-152">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="71b7e-152">alertFeedback</span></span>                                                          | <span data-ttu-id="71b7e-153">Отзыв аналитика об оповещении.</span><span class="sxs-lookup"><span data-stu-id="71b7e-153">Analyst feedback on the alert.</span></span> <span data-ttu-id="71b7e-154">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="71b7e-154">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="71b7e-155">status</span><span class="sxs-lookup"><span data-stu-id="71b7e-155">status</span></span>            | <span data-ttu-id="71b7e-156">alertStatus</span><span class="sxs-lookup"><span data-stu-id="71b7e-156">alertStatus</span></span>                                                            | <span data-ttu-id="71b7e-157">Оповещение состояния жизненного цикла (этап).</span><span class="sxs-lookup"><span data-stu-id="71b7e-157">Alert life cycle status (stage).</span></span> <span data-ttu-id="71b7e-158">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="71b7e-158">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="71b7e-159">tags</span><span class="sxs-lookup"><span data-stu-id="71b7e-159">tags</span></span>              | <span data-ttu-id="71b7e-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71b7e-160">String collection</span></span>                                                      | <span data-ttu-id="71b7e-161">Метки, вызываемые пользователем, которые можно применить к оповещению и могут служить условиями фильтра (например, "HVA", "SAW").</span><span class="sxs-lookup"><span data-stu-id="71b7e-161">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="71b7e-162">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="71b7e-162">vendorInformation</span></span> | [<span data-ttu-id="71b7e-163">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="71b7e-163">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="71b7e-164">Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="71b7e-164">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="71b7e-165">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="71b7e-165">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="71b7e-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b7e-166">Response</span></span>

<span data-ttu-id="71b7e-167">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71b7e-167">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="71b7e-168">Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный объект оповещения `200 OK` в тексте [](../resources/alert.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="71b7e-168">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71b7e-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="71b7e-169">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="71b7e-170">Пример 1. Запрос без загона Prefer</span><span class="sxs-lookup"><span data-stu-id="71b7e-170">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="71b7e-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b7e-171">Request</span></span>

<span data-ttu-id="71b7e-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71b7e-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71b7e-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="71b7e-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="71b7e-174">C#</span><span class="sxs-lookup"><span data-stu-id="71b7e-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71b7e-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71b7e-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71b7e-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71b7e-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71b7e-177">Java</span><span class="sxs-lookup"><span data-stu-id="71b7e-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="71b7e-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b7e-178">Response</span></span>

<span data-ttu-id="71b7e-179">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="71b7e-179">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="71b7e-180">Пример 2. Запрос с помощью загона Prefer</span><span class="sxs-lookup"><span data-stu-id="71b7e-180">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="71b7e-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b7e-181">Request</span></span>

<span data-ttu-id="71b7e-182">В следующем примере показан запрос, который включает заглавную `Prefer` головку запроса.</span><span class="sxs-lookup"><span data-stu-id="71b7e-182">The following example shows a request that includes the `Prefer` request header.</span></span>


# <a name="http"></a>[<span data-ttu-id="71b7e-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="71b7e-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="71b7e-184">C#</span><span class="sxs-lookup"><span data-stu-id="71b7e-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71b7e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71b7e-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71b7e-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71b7e-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71b7e-187">Java</span><span class="sxs-lookup"><span data-stu-id="71b7e-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71b7e-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b7e-188">Response</span></span>

<span data-ttu-id="71b7e-189">Ниже приводится пример ответа, когда используется необязательный `Prefer: return=representation` заглавной запрос.</span><span class="sxs-lookup"><span data-stu-id="71b7e-189">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="71b7e-190">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71b7e-190">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

