---
title: Обновление оповещения
description: Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями. Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d3be1de01e416f7d9ac72c9f3d7d17815c9e6eb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992841"
---
# <a name="update-alert"></a><span data-ttu-id="87839-104">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="87839-104">Update alert</span></span>

<span data-ttu-id="87839-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87839-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87839-106">Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.</span><span class="sxs-lookup"><span data-stu-id="87839-106">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="87839-107">Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="87839-107">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="87839-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87839-108">Permissions</span></span>

<span data-ttu-id="87839-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87839-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87839-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87839-111">Permission type</span></span>                        | <span data-ttu-id="87839-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87839-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="87839-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87839-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="87839-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87839-114">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="87839-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87839-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87839-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87839-116">Not supported.</span></span>                      |
| <span data-ttu-id="87839-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87839-117">Application</span></span>                            | <span data-ttu-id="87839-118">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87839-118">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="87839-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87839-119">HTTP request</span></span>

> <span data-ttu-id="87839-120">**Примечание:** Необходимо включить идентификатор **оповещения** в качестве параметра и вендоринформатион, содержащего `provider` `vendor` метод и с этим методом.</span><span class="sxs-lookup"><span data-stu-id="87839-120">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="87839-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87839-121">Request headers</span></span>

| <span data-ttu-id="87839-122">Имя</span><span class="sxs-lookup"><span data-stu-id="87839-122">Name</span></span>          | <span data-ttu-id="87839-123">Описание</span><span class="sxs-lookup"><span data-stu-id="87839-123">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="87839-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87839-124">Authorization</span></span> | <span data-ttu-id="87839-125">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="87839-125">Bearer {code}.</span></span> <span data-ttu-id="87839-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="87839-126">Required.</span></span> |
| <span data-ttu-id="87839-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="87839-127">Prefer</span></span>        | <span data-ttu-id="87839-128">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="87839-128">return=representation.</span></span> <span data-ttu-id="87839-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="87839-129">Optional.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="87839-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87839-130">Request body</span></span>

<span data-ttu-id="87839-131">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="87839-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="87839-132">Текст **должен** содержать свойство **вендоринформатион** с допустимыми `provider` полями и `vendor` Fields.</span><span class="sxs-lookup"><span data-stu-id="87839-132">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="87839-133">В следующей таблице перечислены поля, которые можно обновить для оповещения.</span><span class="sxs-lookup"><span data-stu-id="87839-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="87839-134">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="87839-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="87839-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="87839-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="87839-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="87839-136">Property</span></span>          | <span data-ttu-id="87839-137">Тип</span><span class="sxs-lookup"><span data-stu-id="87839-137">Type</span></span>                                                                   | <span data-ttu-id="87839-138">Описание</span><span class="sxs-lookup"><span data-stu-id="87839-138">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="87839-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="87839-139">assignedTo</span></span>        | <span data-ttu-id="87839-140">String</span><span class="sxs-lookup"><span data-stu-id="87839-140">String</span></span>                                                                 | <span data-ttu-id="87839-141">Имя аналитика, которому назначено оповещение для рассмотрения, исследования или исправления.</span><span class="sxs-lookup"><span data-stu-id="87839-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="87839-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="87839-142">closedDateTime</span></span>    | <span data-ttu-id="87839-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87839-143">DateTimeOffset</span></span>                                                         | <span data-ttu-id="87839-144">Время закрытия оповещения.</span><span class="sxs-lookup"><span data-stu-id="87839-144">Time at which the alert was closed.</span></span> <span data-ttu-id="87839-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="87839-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87839-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87839-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="87839-147">comments</span><span class="sxs-lookup"><span data-stu-id="87839-147">comments</span></span>          | <span data-ttu-id="87839-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87839-148">String collection</span></span>                                                      | <span data-ttu-id="87839-149">Комментарии аналитика в оповещении (для управления оповещениями клиентов).</span><span class="sxs-lookup"><span data-stu-id="87839-149">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="87839-150">Этот метод может обновить поле Comments только следующими значениями: `Closed in IPC` , `Closed in MCAS` .</span><span class="sxs-lookup"><span data-stu-id="87839-150">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span> |
| <span data-ttu-id="87839-151">feedback</span><span class="sxs-lookup"><span data-stu-id="87839-151">feedback</span></span>          | <span data-ttu-id="87839-152">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="87839-152">alertFeedback</span></span>                                                          | <span data-ttu-id="87839-153">Отзыв аналитика об оповещении.</span><span class="sxs-lookup"><span data-stu-id="87839-153">Analyst feedback on the alert.</span></span> <span data-ttu-id="87839-154">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="87839-154">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="87839-155">status</span><span class="sxs-lookup"><span data-stu-id="87839-155">status</span></span>            | <span data-ttu-id="87839-156">alertStatus</span><span class="sxs-lookup"><span data-stu-id="87839-156">alertStatus</span></span>                                                            | <span data-ttu-id="87839-157">Состояние жизненного цикла оповещений (Stage).</span><span class="sxs-lookup"><span data-stu-id="87839-157">Alert life cycle status (stage).</span></span> <span data-ttu-id="87839-158">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="87839-158">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="87839-159">tags</span><span class="sxs-lookup"><span data-stu-id="87839-159">tags</span></span>              | <span data-ttu-id="87839-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87839-160">String collection</span></span>                                                      | <span data-ttu-id="87839-161">Определяемые пользователями метки, которые могут быть применены к оповещению и могут использоваться в качестве условий фильтрации (например, "Хва", "показано").</span><span class="sxs-lookup"><span data-stu-id="87839-161">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="87839-162">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="87839-162">vendorInformation</span></span> | [<span data-ttu-id="87839-163">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="87839-163">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="87839-164">Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="87839-164">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="87839-165">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="87839-165">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="87839-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="87839-166">Response</span></span>

<span data-ttu-id="87839-167">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="87839-167">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="87839-168">Если используется заголовок необязательного запроса, метод возвращает `200 OK` код отклика и обновленный объект [Alert](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87839-168">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87839-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="87839-169">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="87839-170">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="87839-170">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="87839-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="87839-171">Request</span></span>

<span data-ttu-id="87839-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87839-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87839-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="87839-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
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
# <a name="c"></a>[<span data-ttu-id="87839-174">C#</span><span class="sxs-lookup"><span data-stu-id="87839-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87839-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87839-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87839-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87839-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87839-177">Java</span><span class="sxs-lookup"><span data-stu-id="87839-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="87839-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="87839-178">Response</span></span>

<span data-ttu-id="87839-179">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="87839-179">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="87839-180">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="87839-180">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="87839-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="87839-181">Request</span></span>

<span data-ttu-id="87839-182">В приведенном ниже примере показан запрос, включающий `Prefer` заголовок запроса.</span><span class="sxs-lookup"><span data-stu-id="87839-182">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
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

#### <a name="response"></a><span data-ttu-id="87839-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="87839-183">Response</span></span>

<span data-ttu-id="87839-184">Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.</span><span class="sxs-lookup"><span data-stu-id="87839-184">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="87839-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87839-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

