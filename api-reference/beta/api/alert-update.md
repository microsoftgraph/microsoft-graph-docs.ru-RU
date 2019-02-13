---
title: Обновление оповещения
description: Обновите редактируемых свойств оповещения в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b1fec6bfca2ce116bc35c4a7c8a115418b15012
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967328"
---
# <a name="update-alert"></a><span data-ttu-id="3c830-103">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="3c830-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c830-104">Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.</span><span class="sxs-lookup"><span data-stu-id="3c830-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="3c830-105">Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3c830-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c830-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c830-106">Permissions</span></span>

<span data-ttu-id="3c830-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c830-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c830-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c830-109">Permission type</span></span>      | <span data-ttu-id="3c830-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c830-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c830-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c830-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="3c830-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c830-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="3c830-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c830-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3c830-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c830-114">Not supported.</span></span>  |
|<span data-ttu-id="3c830-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c830-115">Application</span></span> | <span data-ttu-id="3c830-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c830-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c830-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c830-117">HTTP request</span></span>

> <span data-ttu-id="3c830-118">**Примечание:** Необходимо указать код **оповещение о** как параметр и содержащий vendorInformation `provider` и `vendor` с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c830-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="3c830-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c830-119">Request headers</span></span>

| <span data-ttu-id="3c830-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3c830-120">Name</span></span>       | <span data-ttu-id="3c830-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3c830-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3c830-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c830-122">Authorization</span></span>  | <span data-ttu-id="3c830-p103">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c830-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="3c830-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="3c830-125">Prefer</span></span> | <span data-ttu-id="3c830-126">Возвращает = представление</span><span class="sxs-lookup"><span data-stu-id="3c830-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c830-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c830-127">Request body</span></span>

<span data-ttu-id="3c830-128">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="3c830-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3c830-129">Текст, **должны** содержать `vendorInformation` свойство с допустимыми `provider` и `vendor` полей.</span><span class="sxs-lookup"><span data-stu-id="3c830-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="3c830-130">В следующей таблице приведены поля, которые могут быть обновлены для оповещения.</span><span class="sxs-lookup"><span data-stu-id="3c830-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="3c830-131">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="3c830-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="3c830-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3c830-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c830-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c830-133">Property</span></span>   | <span data-ttu-id="3c830-134">Тип</span><span class="sxs-lookup"><span data-stu-id="3c830-134">Type</span></span> |<span data-ttu-id="3c830-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3c830-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c830-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3c830-136">assignedTo</span></span>|<span data-ttu-id="3c830-137">String</span><span class="sxs-lookup"><span data-stu-id="3c830-137">String</span></span>|<span data-ttu-id="3c830-138">Имя аналитик оповещение будет назначен для рассмотрения исследования и исправления.</span><span class="sxs-lookup"><span data-stu-id="3c830-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="3c830-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c830-139">closedDateTime</span></span>|<span data-ttu-id="3c830-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c830-140">DateTimeOffset</span></span>|<span data-ttu-id="3c830-141">Время закрытия оповещение.</span><span class="sxs-lookup"><span data-stu-id="3c830-141">Time at which the alert was closed.</span></span> <span data-ttu-id="3c830-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3c830-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c830-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3c830-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3c830-144">comments</span><span class="sxs-lookup"><span data-stu-id="3c830-144">comments</span></span>|<span data-ttu-id="3c830-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3c830-145">String collection</span></span>|<span data-ttu-id="3c830-146">Комментарии аналитик оповещения (для управления предупреждениями клиента).</span><span class="sxs-lookup"><span data-stu-id="3c830-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="3c830-147">свои отзывы и предложения</span><span class="sxs-lookup"><span data-stu-id="3c830-147">feedback</span></span>|<span data-ttu-id="3c830-148">Перечисление alertFeedback</span><span class="sxs-lookup"><span data-stu-id="3c830-148">alertFeedback enum</span></span>|<span data-ttu-id="3c830-149">Отзыв аналитик на оповещение.</span><span class="sxs-lookup"><span data-stu-id="3c830-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="3c830-150">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="3c830-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="3c830-151">status</span><span class="sxs-lookup"><span data-stu-id="3c830-151">status</span></span>|<span data-ttu-id="3c830-152">Перечисление alertStatus</span><span class="sxs-lookup"><span data-stu-id="3c830-152">alertStatus enum</span></span>|<span data-ttu-id="3c830-153">Состояние оповещений жизненного цикла (рабочей области).</span><span class="sxs-lookup"><span data-stu-id="3c830-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="3c830-154">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="3c830-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="3c830-155">tags</span><span class="sxs-lookup"><span data-stu-id="3c830-155">tags</span></span>|<span data-ttu-id="3c830-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c830-156">String collection</span></span>|<span data-ttu-id="3c830-157">Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например, «HVA», «ЗАФИКСИРОВАЛА).</span><span class="sxs-lookup"><span data-stu-id="3c830-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="3c830-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="3c830-158">vendorInformation</span></span> |[<span data-ttu-id="3c830-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="3c830-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="3c830-160">Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="3c830-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="3c830-161">**Поставщик и поставщика поля являются обязательными.**</span><span class="sxs-lookup"><span data-stu-id="3c830-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="3c830-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c830-162">Response</span></span>

<span data-ttu-id="3c830-163">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c830-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="3c830-164">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и объект обновленные [оповещения](../resources/alert.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c830-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c830-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c830-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="3c830-166">В примере 1: Запрос без Prefer заголовка</span><span class="sxs-lookup"><span data-stu-id="3c830-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="3c830-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c830-167">Request</span></span>

<span data-ttu-id="3c830-168">Ниже приведен пример запроса без `Prefer` заголовка.</span><span class="sxs-lookup"><span data-stu-id="3c830-168">The following is an example of the request without the `Prefer` header.</span></span>
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

#### <a name="response"></a><span data-ttu-id="3c830-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c830-169">Response</span></span>

<span data-ttu-id="3c830-170">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="3c830-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="3c830-171">Пример 2: Запрос с заголовком, Prefer</span><span class="sxs-lookup"><span data-stu-id="3c830-171">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="3c830-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c830-172">Request</span></span>

<span data-ttu-id="3c830-173">В следующем примере показан запрос, который включает в себя `Prefer` заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="3c830-173">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="3c830-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c830-174">Response</span></span>

<span data-ttu-id="3c830-175">Ниже приведен пример ответа при Дополнительно `Prefer: return=representation` используется заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="3c830-175">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="3c830-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c830-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
