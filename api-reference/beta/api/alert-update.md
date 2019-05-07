---
title: Обновление оповещения
description: Обновление редактируемого свойства оповещения в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: de663b4cdcd4f12bfdf3d180f039144f86d2d624
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636564"
---
# <a name="update-alert"></a><span data-ttu-id="14c75-103">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="14c75-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14c75-104">Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.</span><span class="sxs-lookup"><span data-stu-id="14c75-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="14c75-105">Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="14c75-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="14c75-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14c75-106">Permissions</span></span>

<span data-ttu-id="14c75-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14c75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14c75-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14c75-109">Permission type</span></span>      | <span data-ttu-id="14c75-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14c75-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14c75-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14c75-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="14c75-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c75-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="14c75-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14c75-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="14c75-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14c75-114">Not supported.</span></span>  |
|<span data-ttu-id="14c75-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14c75-115">Application</span></span> | <span data-ttu-id="14c75-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c75-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14c75-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14c75-117">HTTP request</span></span>

> <span data-ttu-id="14c75-118">**Примечание:** Необходимо включить идентификатор **оповещения** в качестве параметра и вендоринформатион, содержащего метод `provider` и `vendor` с этим методом.</span><span class="sxs-lookup"><span data-stu-id="14c75-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="14c75-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14c75-119">Request headers</span></span>

| <span data-ttu-id="14c75-120">Имя</span><span class="sxs-lookup"><span data-stu-id="14c75-120">Name</span></span>       | <span data-ttu-id="14c75-121">Описание</span><span class="sxs-lookup"><span data-stu-id="14c75-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="14c75-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14c75-122">Authorization</span></span>  | <span data-ttu-id="14c75-123">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="14c75-123">Bearer {code}.</span></span> <span data-ttu-id="14c75-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="14c75-124">Required.</span></span>|
|<span data-ttu-id="14c75-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="14c75-125">Prefer</span></span> | <span data-ttu-id="14c75-126">Возврат = представление</span><span class="sxs-lookup"><span data-stu-id="14c75-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="14c75-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14c75-127">Request body</span></span>

<span data-ttu-id="14c75-128">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="14c75-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="14c75-129">Текст **должен** содержать `vendorInformation` свойство Valid `provider` и `vendor` Fields.</span><span class="sxs-lookup"><span data-stu-id="14c75-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="14c75-130">В следующей таблице перечислены поля, которые можно обновить для оповещения.</span><span class="sxs-lookup"><span data-stu-id="14c75-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="14c75-131">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="14c75-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="14c75-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="14c75-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="14c75-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="14c75-133">Property</span></span>   | <span data-ttu-id="14c75-134">Тип</span><span class="sxs-lookup"><span data-stu-id="14c75-134">Type</span></span> |<span data-ttu-id="14c75-135">Описание</span><span class="sxs-lookup"><span data-stu-id="14c75-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14c75-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="14c75-136">assignedTo</span></span>|<span data-ttu-id="14c75-137">String</span><span class="sxs-lookup"><span data-stu-id="14c75-137">String</span></span>|<span data-ttu-id="14c75-138">Имя аналитика, которому назначено оповещение для рассмотрения, исследования или исправления.</span><span class="sxs-lookup"><span data-stu-id="14c75-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="14c75-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="14c75-139">closedDateTime</span></span>|<span data-ttu-id="14c75-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14c75-140">DateTimeOffset</span></span>|<span data-ttu-id="14c75-141">Время закрытия оповещения.</span><span class="sxs-lookup"><span data-stu-id="14c75-141">Time at which the alert was closed.</span></span> <span data-ttu-id="14c75-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="14c75-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14c75-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="14c75-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="14c75-144">comments</span><span class="sxs-lookup"><span data-stu-id="14c75-144">comments</span></span>|<span data-ttu-id="14c75-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14c75-145">String collection</span></span>|<span data-ttu-id="14c75-146">Комментарии аналитика в оповещении (для управления оповещениями клиентов).</span><span class="sxs-lookup"><span data-stu-id="14c75-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="14c75-147">feedback</span><span class="sxs-lookup"><span data-stu-id="14c75-147">feedback</span></span>|<span data-ttu-id="14c75-148">Перечисление Алертфидбакк</span><span class="sxs-lookup"><span data-stu-id="14c75-148">alertFeedback enum</span></span>|<span data-ttu-id="14c75-149">Отзыв аналитика об оповещении.</span><span class="sxs-lookup"><span data-stu-id="14c75-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="14c75-150">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="14c75-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="14c75-151">status</span><span class="sxs-lookup"><span data-stu-id="14c75-151">status</span></span>|<span data-ttu-id="14c75-152">Перечисление Алертстатус</span><span class="sxs-lookup"><span data-stu-id="14c75-152">alertStatus enum</span></span>|<span data-ttu-id="14c75-153">Состояние жизненного цикла оповещений (Stage).</span><span class="sxs-lookup"><span data-stu-id="14c75-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="14c75-154">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="14c75-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="14c75-155">tags</span><span class="sxs-lookup"><span data-stu-id="14c75-155">tags</span></span>|<span data-ttu-id="14c75-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14c75-156">String collection</span></span>|<span data-ttu-id="14c75-157">Определяемые пользователями метки, которые могут быть применены к оповещению и могут использоваться в качестве условий фильтрации (например, "Хва", "показано").</span><span class="sxs-lookup"><span data-stu-id="14c75-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="14c75-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="14c75-158">vendorInformation</span></span> |[<span data-ttu-id="14c75-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="14c75-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="14c75-160">Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="14c75-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="14c75-161">**Требуются поля поставщика и поставщика.**</span><span class="sxs-lookup"><span data-stu-id="14c75-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="14c75-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="14c75-162">Response</span></span>

<span data-ttu-id="14c75-163">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14c75-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="14c75-164">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [Alert](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14c75-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14c75-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="14c75-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="14c75-166">Пример 1: запрос без верхнего колонтитула</span><span class="sxs-lookup"><span data-stu-id="14c75-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="14c75-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="14c75-167">Request</span></span>

<span data-ttu-id="14c75-168">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="14c75-168">The following is an example of the request without the `Prefer` header.</span></span>
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

#### <a name="response"></a><span data-ttu-id="14c75-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="14c75-169">Response</span></span>

<span data-ttu-id="14c75-170">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="14c75-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="14c75-171">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="14c75-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="14c75-172">Языках</span><span class="sxs-lookup"><span data-stu-id="14c75-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14c75-173">Язык</span><span class="sxs-lookup"><span data-stu-id="14c75-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_alert-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="14c75-174">Пример 2: запрос с заголовком предпочтения</span><span class="sxs-lookup"><span data-stu-id="14c75-174">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="14c75-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="14c75-175">Request</span></span>

<span data-ttu-id="14c75-176">В приведенном ниже примере показан запрос, включающий заголовок `Prefer` запроса.</span><span class="sxs-lookup"><span data-stu-id="14c75-176">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="14c75-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="14c75-177">Response</span></span>

<span data-ttu-id="14c75-178">Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.</span><span class="sxs-lookup"><span data-stu-id="14c75-178">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="14c75-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14c75-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
