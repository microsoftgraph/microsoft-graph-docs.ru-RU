---
title: Обновление оповещения
description: Обновление редактируемого свойства оповещения в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3ad81e698c43e8863d3081d6995fc29b1b9a9dc3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258543"
---
# <a name="update-alert"></a><span data-ttu-id="698cd-103">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="698cd-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="698cd-104">Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.</span><span class="sxs-lookup"><span data-stu-id="698cd-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="698cd-105">Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="698cd-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="698cd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="698cd-106">Permissions</span></span>

<span data-ttu-id="698cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="698cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="698cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="698cd-109">Permission type</span></span>      | <span data-ttu-id="698cd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="698cd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="698cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="698cd-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="698cd-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698cd-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="698cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="698cd-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="698cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="698cd-114">Not supported.</span></span>  |
|<span data-ttu-id="698cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="698cd-115">Application</span></span> | <span data-ttu-id="698cd-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="698cd-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="698cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="698cd-117">HTTP request</span></span>

> <span data-ttu-id="698cd-118">**Примечание:** Необходимо включить идентификатор **оповещения** в качестве параметра и вендоринформатион, содержащего метод `provider` и `vendor` с этим методом.</span><span class="sxs-lookup"><span data-stu-id="698cd-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="698cd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="698cd-119">Request headers</span></span>

| <span data-ttu-id="698cd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="698cd-120">Name</span></span>       | <span data-ttu-id="698cd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="698cd-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="698cd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="698cd-122">Authorization</span></span>  | <span data-ttu-id="698cd-123">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="698cd-123">Bearer {code}.</span></span> <span data-ttu-id="698cd-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="698cd-124">Required.</span></span>|
|<span data-ttu-id="698cd-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="698cd-125">Prefer</span></span> | <span data-ttu-id="698cd-126">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="698cd-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="698cd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="698cd-127">Request body</span></span>

<span data-ttu-id="698cd-128">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="698cd-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="698cd-129">Текст **должен** содержать `vendorInformation` свойство Valid `provider` и `vendor` Fields.</span><span class="sxs-lookup"><span data-stu-id="698cd-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="698cd-130">В следующей таблице перечислены поля, которые можно обновить для оповещения.</span><span class="sxs-lookup"><span data-stu-id="698cd-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="698cd-131">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="698cd-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="698cd-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="698cd-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="698cd-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="698cd-133">Property</span></span>   | <span data-ttu-id="698cd-134">Тип</span><span class="sxs-lookup"><span data-stu-id="698cd-134">Type</span></span> |<span data-ttu-id="698cd-135">Описание</span><span class="sxs-lookup"><span data-stu-id="698cd-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="698cd-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="698cd-136">assignedTo</span></span>|<span data-ttu-id="698cd-137">String</span><span class="sxs-lookup"><span data-stu-id="698cd-137">String</span></span>|<span data-ttu-id="698cd-138">Имя аналитика, которому назначено оповещение для рассмотрения, исследования или исправления.</span><span class="sxs-lookup"><span data-stu-id="698cd-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="698cd-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="698cd-139">closedDateTime</span></span>|<span data-ttu-id="698cd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="698cd-140">DateTimeOffset</span></span>|<span data-ttu-id="698cd-141">Время закрытия оповещения.</span><span class="sxs-lookup"><span data-stu-id="698cd-141">Time at which the alert was closed.</span></span> <span data-ttu-id="698cd-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="698cd-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="698cd-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="698cd-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="698cd-144">comments</span><span class="sxs-lookup"><span data-stu-id="698cd-144">comments</span></span>|<span data-ttu-id="698cd-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="698cd-145">String collection</span></span>|<span data-ttu-id="698cd-146">Комментарии аналитика в оповещении (для управления оповещениями клиентов).</span><span class="sxs-lookup"><span data-stu-id="698cd-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="698cd-147">feedback</span><span class="sxs-lookup"><span data-stu-id="698cd-147">feedback</span></span>|<span data-ttu-id="698cd-148">Перечисление Алертфидбакк</span><span class="sxs-lookup"><span data-stu-id="698cd-148">alertFeedback enum</span></span>|<span data-ttu-id="698cd-149">Отзыв аналитика об оповещении.</span><span class="sxs-lookup"><span data-stu-id="698cd-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="698cd-150">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="698cd-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="698cd-151">status</span><span class="sxs-lookup"><span data-stu-id="698cd-151">status</span></span>|<span data-ttu-id="698cd-152">Перечисление Алертстатус</span><span class="sxs-lookup"><span data-stu-id="698cd-152">alertStatus enum</span></span>|<span data-ttu-id="698cd-153">Состояние жизненного цикла оповещений (Stage).</span><span class="sxs-lookup"><span data-stu-id="698cd-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="698cd-154">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="698cd-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="698cd-155">tags</span><span class="sxs-lookup"><span data-stu-id="698cd-155">tags</span></span>|<span data-ttu-id="698cd-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="698cd-156">String collection</span></span>|<span data-ttu-id="698cd-157">Определяемые пользователями метки, которые могут быть применены к оповещению и могут использоваться в качестве условий фильтрации (например, "Хва", "показано").</span><span class="sxs-lookup"><span data-stu-id="698cd-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="698cd-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="698cd-158">vendorInformation</span></span> |[<span data-ttu-id="698cd-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="698cd-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="698cd-160">Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="698cd-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="698cd-161">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="698cd-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="698cd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="698cd-162">Response</span></span>

<span data-ttu-id="698cd-163">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="698cd-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="698cd-164">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [Alert](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="698cd-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="698cd-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="698cd-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="698cd-166">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="698cd-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="698cd-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="698cd-167">Request</span></span>

<span data-ttu-id="698cd-168">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="698cd-168">The following is an example of the request without the `Prefer` header.</span></span>
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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="698cd-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="698cd-169">Response</span></span>

<span data-ttu-id="698cd-170">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="698cd-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="698cd-171">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="698cd-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="698cd-172">C#</span><span class="sxs-lookup"><span data-stu-id="698cd-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="698cd-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="698cd-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_alert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="698cd-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="698cd-174">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_alert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="698cd-175">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="698cd-175">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="698cd-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="698cd-176">Request</span></span>

<span data-ttu-id="698cd-177">В приведенном ниже примере показан запрос, включающий заголовок `Prefer` запроса.</span><span class="sxs-lookup"><span data-stu-id="698cd-177">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="698cd-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="698cd-178">Response</span></span>

<span data-ttu-id="698cd-179">Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.</span><span class="sxs-lookup"><span data-stu-id="698cd-179">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="698cd-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="698cd-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
