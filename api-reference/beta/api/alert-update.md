---
title: Обновление оповещения
description: Обновление редактируемого свойства оповещения в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1caf9c4bd9f0e117743f615ad991cdeffeb2b702
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962331"
---
# <a name="update-alert"></a><span data-ttu-id="477eb-103">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="477eb-103">Update alert</span></span>

<span data-ttu-id="477eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="477eb-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="477eb-105">Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.</span><span class="sxs-lookup"><span data-stu-id="477eb-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="477eb-106">Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="477eb-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="477eb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="477eb-107">Permissions</span></span>

<span data-ttu-id="477eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="477eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="477eb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="477eb-110">Permission type</span></span>      | <span data-ttu-id="477eb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="477eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="477eb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="477eb-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="477eb-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477eb-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="477eb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="477eb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="477eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="477eb-115">Not supported.</span></span>  |
|<span data-ttu-id="477eb-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="477eb-116">Application</span></span> | <span data-ttu-id="477eb-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477eb-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="477eb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="477eb-118">HTTP request</span></span>

> <span data-ttu-id="477eb-119">**Примечание:** Необходимо включить идентификатор **оповещения** в качестве параметра и вендоринформатион, содержащего `provider` `vendor` метод и с этим методом.</span><span class="sxs-lookup"><span data-stu-id="477eb-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="477eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="477eb-120">Request headers</span></span>

| <span data-ttu-id="477eb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="477eb-121">Name</span></span>       | <span data-ttu-id="477eb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="477eb-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="477eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="477eb-123">Authorization</span></span>  | <span data-ttu-id="477eb-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="477eb-124">Bearer {code}.</span></span> <span data-ttu-id="477eb-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="477eb-125">Required.</span></span>|
|<span data-ttu-id="477eb-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="477eb-126">Prefer</span></span> | <span data-ttu-id="477eb-127">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="477eb-127">return=representation.</span></span> <span data-ttu-id="477eb-128">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="477eb-128">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="477eb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="477eb-129">Request body</span></span>

<span data-ttu-id="477eb-130">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="477eb-130">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="477eb-131">Текст **должен** содержать свойство **вендоринформатион** с допустимыми `provider` полями и `vendor` Fields.</span><span class="sxs-lookup"><span data-stu-id="477eb-131">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="477eb-132">В следующей таблице перечислены поля, которые можно обновить для оповещения.</span><span class="sxs-lookup"><span data-stu-id="477eb-132">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="477eb-133">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="477eb-133">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="477eb-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="477eb-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="477eb-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="477eb-135">Property</span></span>   | <span data-ttu-id="477eb-136">Тип</span><span class="sxs-lookup"><span data-stu-id="477eb-136">Type</span></span> |<span data-ttu-id="477eb-137">Описание</span><span class="sxs-lookup"><span data-stu-id="477eb-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="477eb-138">assignedTo</span><span class="sxs-lookup"><span data-stu-id="477eb-138">assignedTo</span></span>|<span data-ttu-id="477eb-139">String</span><span class="sxs-lookup"><span data-stu-id="477eb-139">String</span></span>|<span data-ttu-id="477eb-140">Имя аналитика, которому назначено оповещение для рассмотрения, исследования или исправления.</span><span class="sxs-lookup"><span data-stu-id="477eb-140">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="477eb-141">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="477eb-141">closedDateTime</span></span>|<span data-ttu-id="477eb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="477eb-142">DateTimeOffset</span></span>|<span data-ttu-id="477eb-143">Время закрытия оповещения.</span><span class="sxs-lookup"><span data-stu-id="477eb-143">Time at which the alert was closed.</span></span> <span data-ttu-id="477eb-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="477eb-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="477eb-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="477eb-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="477eb-146">comments</span><span class="sxs-lookup"><span data-stu-id="477eb-146">comments</span></span>|<span data-ttu-id="477eb-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="477eb-147">String collection</span></span>|<span data-ttu-id="477eb-148">Комментарии аналитика в оповещении (для управления оповещениями клиентов).</span><span class="sxs-lookup"><span data-stu-id="477eb-148">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="477eb-149">Этот метод может обновить поле Comments только следующими значениями: `Closed in IPC` , `Closed in MCAS` .</span><span class="sxs-lookup"><span data-stu-id="477eb-149">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span>|
|<span data-ttu-id="477eb-150">feedback</span><span class="sxs-lookup"><span data-stu-id="477eb-150">feedback</span></span>|<span data-ttu-id="477eb-151">Перечисление Алертфидбакк</span><span class="sxs-lookup"><span data-stu-id="477eb-151">alertFeedback enum</span></span>|<span data-ttu-id="477eb-152">Отзыв аналитика об оповещении.</span><span class="sxs-lookup"><span data-stu-id="477eb-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="477eb-153">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="477eb-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="477eb-154">status</span><span class="sxs-lookup"><span data-stu-id="477eb-154">status</span></span>|<span data-ttu-id="477eb-155">Перечисление Алертстатус</span><span class="sxs-lookup"><span data-stu-id="477eb-155">alertStatus enum</span></span>|<span data-ttu-id="477eb-156">Состояние жизненного цикла оповещений (Stage).</span><span class="sxs-lookup"><span data-stu-id="477eb-156">Alert life cycle status (stage).</span></span> <span data-ttu-id="477eb-157">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="477eb-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="477eb-158">tags</span><span class="sxs-lookup"><span data-stu-id="477eb-158">tags</span></span>|<span data-ttu-id="477eb-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="477eb-159">String collection</span></span>|<span data-ttu-id="477eb-160">Определяемые пользователями метки, которые могут быть применены к оповещению и могут использоваться в качестве условий фильтрации (например, "Хва", "показано").</span><span class="sxs-lookup"><span data-stu-id="477eb-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="477eb-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="477eb-161">vendorInformation</span></span> |[<span data-ttu-id="477eb-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="477eb-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="477eb-163">Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="477eb-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="477eb-164">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="477eb-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="477eb-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="477eb-165">Response</span></span>

<span data-ttu-id="477eb-166">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="477eb-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="477eb-167">Если используется заголовок необязательного запроса, метод возвращает `200 OK` код отклика и обновленный объект [Alert](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="477eb-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="477eb-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="477eb-168">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="477eb-169">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="477eb-169">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="477eb-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="477eb-170">Request</span></span>

<span data-ttu-id="477eb-171">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="477eb-171">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="477eb-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="477eb-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="477eb-173">C#</span><span class="sxs-lookup"><span data-stu-id="477eb-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="477eb-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="477eb-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="477eb-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="477eb-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="477eb-176">Java</span><span class="sxs-lookup"><span data-stu-id="477eb-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="477eb-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="477eb-177">Response</span></span>

<span data-ttu-id="477eb-178">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="477eb-178">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="477eb-179">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="477eb-179">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="477eb-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="477eb-180">Request</span></span>

<span data-ttu-id="477eb-181">В приведенном ниже примере показан запрос, включающий `Prefer` заголовок запроса.</span><span class="sxs-lookup"><span data-stu-id="477eb-181">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a><span data-ttu-id="477eb-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="477eb-182">Response</span></span>

<span data-ttu-id="477eb-183">Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.</span><span class="sxs-lookup"><span data-stu-id="477eb-183">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="477eb-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="477eb-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


