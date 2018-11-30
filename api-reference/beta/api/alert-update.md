---
title: обновление оповещения.
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 9f8040220c64310a04293d43c0c31704c3f49261
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2018
ms.locfileid: "27082894"
---
# <a name="update-alert"></a><span data-ttu-id="809e2-104">обновление оповещения.</span><span class="sxs-lookup"><span data-stu-id="809e2-104">Update alert</span></span>

 > <span data-ttu-id="809e2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="809e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="809e2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="809e2-107">Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.</span><span class="sxs-lookup"><span data-stu-id="809e2-107">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="809e2-108">Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="809e2-108">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="809e2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="809e2-109">Permissions</span></span>

<span data-ttu-id="809e2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="809e2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="809e2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="809e2-112">Permission type</span></span>      | <span data-ttu-id="809e2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="809e2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="809e2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="809e2-114">Delegated (work or school account)</span></span> |   <span data-ttu-id="809e2-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809e2-115">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="809e2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="809e2-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="809e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809e2-117">Not supported.</span></span>  |
|<span data-ttu-id="809e2-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="809e2-118">Application</span></span> | <span data-ttu-id="809e2-119">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809e2-119">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="809e2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="809e2-120">HTTP request</span></span>

> <span data-ttu-id="809e2-121">**Примечание:** Необходимо указать код **оповещение о** как параметр и содержащий vendorInformation `provider` и `vendor` с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="809e2-121">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="809e2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="809e2-122">Request headers</span></span>

| <span data-ttu-id="809e2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="809e2-123">Name</span></span>       | <span data-ttu-id="809e2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="809e2-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="809e2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="809e2-125">Authorization</span></span>  | <span data-ttu-id="809e2-p105">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="809e2-p105">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="809e2-128">Prefer</span><span class="sxs-lookup"><span data-stu-id="809e2-128">Prefer</span></span> | <span data-ttu-id="809e2-129">Возвращает = представление</span><span class="sxs-lookup"><span data-stu-id="809e2-129">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="809e2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="809e2-130">Request body</span></span>

<span data-ttu-id="809e2-131">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="809e2-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="809e2-132">Текст, **должны** содержать `vendorInformation` свойство с допустимыми `provider` и `vendor` полей.</span><span class="sxs-lookup"><span data-stu-id="809e2-132">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="809e2-133">В следующей таблице приведены поля, которые могут быть обновлены для оповещения.</span><span class="sxs-lookup"><span data-stu-id="809e2-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="809e2-134">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="809e2-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="809e2-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="809e2-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="809e2-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="809e2-136">Property</span></span>   | <span data-ttu-id="809e2-137">Тип</span><span class="sxs-lookup"><span data-stu-id="809e2-137">Type</span></span> |<span data-ttu-id="809e2-138">Description</span><span class="sxs-lookup"><span data-stu-id="809e2-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="809e2-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="809e2-139">assignedTo</span></span>|<span data-ttu-id="809e2-140">String</span><span class="sxs-lookup"><span data-stu-id="809e2-140">String</span></span>|<span data-ttu-id="809e2-141">Имя аналитик оповещение будет назначен для рассмотрения исследования и исправления.</span><span class="sxs-lookup"><span data-stu-id="809e2-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="809e2-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="809e2-142">closedDateTime</span></span>|<span data-ttu-id="809e2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809e2-143">DateTimeOffset</span></span>|<span data-ttu-id="809e2-144">Время закрытия оповещение.</span><span class="sxs-lookup"><span data-stu-id="809e2-144">Time at which the alert was closed.</span></span> <span data-ttu-id="809e2-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="809e2-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="809e2-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="809e2-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="809e2-147">comments</span><span class="sxs-lookup"><span data-stu-id="809e2-147">comments</span></span>|<span data-ttu-id="809e2-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="809e2-148">String collection</span></span>|<span data-ttu-id="809e2-149">Комментарии аналитик оповещения (для управления предупреждениями клиента).</span><span class="sxs-lookup"><span data-stu-id="809e2-149">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="809e2-150">свои отзывы и предложения</span><span class="sxs-lookup"><span data-stu-id="809e2-150">feedback</span></span>|<span data-ttu-id="809e2-151">Перечисление alertFeedback</span><span class="sxs-lookup"><span data-stu-id="809e2-151">alertFeedback enum</span></span>|<span data-ttu-id="809e2-152">Отзыв аналитик на оповещение.</span><span class="sxs-lookup"><span data-stu-id="809e2-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="809e2-153">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="809e2-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="809e2-154">status</span><span class="sxs-lookup"><span data-stu-id="809e2-154">status</span></span>|<span data-ttu-id="809e2-155">Перечисление alertStatus</span><span class="sxs-lookup"><span data-stu-id="809e2-155">alertStatus enum</span></span>|<span data-ttu-id="809e2-156">Состояние оповещений жизненного цикла (рабочей области).</span><span class="sxs-lookup"><span data-stu-id="809e2-156">Alert lifecycle status (stage).</span></span> <span data-ttu-id="809e2-157">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="809e2-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="809e2-158">теги</span><span class="sxs-lookup"><span data-stu-id="809e2-158">tags</span></span>|<span data-ttu-id="809e2-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="809e2-159">String collection</span></span>|<span data-ttu-id="809e2-160">Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например, «HVA», «ЗАФИКСИРОВАЛА).</span><span class="sxs-lookup"><span data-stu-id="809e2-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="809e2-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="809e2-161">vendorInformation</span></span> |[<span data-ttu-id="809e2-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="809e2-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="809e2-163">Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="809e2-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="809e2-164">**Поставщик и поставщика поля являются обязательными.**</span><span class="sxs-lookup"><span data-stu-id="809e2-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="809e2-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="809e2-165">Response</span></span>

<span data-ttu-id="809e2-166">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="809e2-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="809e2-167">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и объект обновленные [оповещения](../resources/alert.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="809e2-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="809e2-168">Пример 1</span><span class="sxs-lookup"><span data-stu-id="809e2-168">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="809e2-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="809e2-169">Request</span></span>

<span data-ttu-id="809e2-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="809e2-170">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="809e2-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="809e2-171">Response</span></span>

<span data-ttu-id="809e2-172">Ниже приведен пример успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="809e2-172">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="809e2-173">Пример 2</span><span class="sxs-lookup"><span data-stu-id="809e2-173">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="809e2-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="809e2-174">Request</span></span>

<span data-ttu-id="809e2-175">В следующем примере показан запрос, который включает в себя `Prefer` заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="809e2-175">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="809e2-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="809e2-176">Response</span></span>

<span data-ttu-id="809e2-177">Ниже приведен пример ответа при Дополнительно `Prefer: return=representation` используется заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="809e2-177">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="809e2-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="809e2-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
