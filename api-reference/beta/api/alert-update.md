---
title: обновление оповещения.
description: Обновите редактируемых свойств оповещения в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fc0bc88dad83024d3da2d6f2adf3f16288719cb2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517416"
---
# <a name="update-alert"></a><span data-ttu-id="c8583-103">обновление оповещения.</span><span class="sxs-lookup"><span data-stu-id="c8583-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8583-104">Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.</span><span class="sxs-lookup"><span data-stu-id="c8583-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="c8583-105">Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="c8583-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8583-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8583-106">Permissions</span></span>

<span data-ttu-id="c8583-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8583-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8583-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8583-109">Permission type</span></span>      | <span data-ttu-id="c8583-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8583-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8583-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8583-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="c8583-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8583-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="c8583-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8583-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c8583-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8583-114">Not supported.</span></span>  |
|<span data-ttu-id="c8583-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8583-115">Application</span></span> | <span data-ttu-id="c8583-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8583-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8583-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8583-117">HTTP request</span></span>

> <span data-ttu-id="c8583-118">**Примечание:** Необходимо указать код **оповещение о** как параметр и содержащий vendorInformation `provider` и `vendor` с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8583-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="c8583-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8583-119">Request headers</span></span>

| <span data-ttu-id="c8583-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8583-120">Name</span></span>       | <span data-ttu-id="c8583-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c8583-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c8583-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8583-122">Authorization</span></span>  | <span data-ttu-id="c8583-p103">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8583-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="c8583-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="c8583-125">Prefer</span></span> | <span data-ttu-id="c8583-126">Возвращает = представление</span><span class="sxs-lookup"><span data-stu-id="c8583-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8583-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8583-127">Request body</span></span>

<span data-ttu-id="c8583-128">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="c8583-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c8583-129">Текст, **должны** содержать `vendorInformation` свойство с допустимыми `provider` и `vendor` полей.</span><span class="sxs-lookup"><span data-stu-id="c8583-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="c8583-130">В следующей таблице приведены поля, которые могут быть обновлены для оповещения.</span><span class="sxs-lookup"><span data-stu-id="c8583-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="c8583-131">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="c8583-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="c8583-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c8583-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8583-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8583-133">Property</span></span>   | <span data-ttu-id="c8583-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c8583-134">Type</span></span> |<span data-ttu-id="c8583-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c8583-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8583-136">AssignedTo</span><span class="sxs-lookup"><span data-stu-id="c8583-136">assignedTo</span></span>|<span data-ttu-id="c8583-137">String</span><span class="sxs-lookup"><span data-stu-id="c8583-137">String</span></span>|<span data-ttu-id="c8583-138">Имя аналитик оповещение будет назначен для рассмотрения исследования и исправления.</span><span class="sxs-lookup"><span data-stu-id="c8583-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="c8583-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8583-139">closedDateTime</span></span>|<span data-ttu-id="c8583-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8583-140">DateTimeOffset</span></span>|<span data-ttu-id="c8583-141">Время закрытия оповещение.</span><span class="sxs-lookup"><span data-stu-id="c8583-141">Time at which the alert was closed.</span></span> <span data-ttu-id="c8583-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c8583-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c8583-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c8583-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c8583-144">comments</span><span class="sxs-lookup"><span data-stu-id="c8583-144">comments</span></span>|<span data-ttu-id="c8583-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8583-145">String collection</span></span>|<span data-ttu-id="c8583-146">Комментарии аналитик оповещения (для управления предупреждениями клиента).</span><span class="sxs-lookup"><span data-stu-id="c8583-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="c8583-147">Отзывы</span><span class="sxs-lookup"><span data-stu-id="c8583-147">feedback</span></span>|<span data-ttu-id="c8583-148">Перечисление alertFeedback</span><span class="sxs-lookup"><span data-stu-id="c8583-148">alertFeedback enum</span></span>|<span data-ttu-id="c8583-149">Отзыв аналитик на оповещение.</span><span class="sxs-lookup"><span data-stu-id="c8583-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="c8583-150">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="c8583-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="c8583-151">status</span><span class="sxs-lookup"><span data-stu-id="c8583-151">status</span></span>|<span data-ttu-id="c8583-152">Перечисление alertStatus</span><span class="sxs-lookup"><span data-stu-id="c8583-152">alertStatus enum</span></span>|<span data-ttu-id="c8583-153">Состояние оповещений жизненного цикла (рабочей области).</span><span class="sxs-lookup"><span data-stu-id="c8583-153">Alert lifecycle status (stage).</span></span> <span data-ttu-id="c8583-154">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="c8583-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="c8583-155">tags</span><span class="sxs-lookup"><span data-stu-id="c8583-155">tags</span></span>|<span data-ttu-id="c8583-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8583-156">String collection</span></span>|<span data-ttu-id="c8583-157">Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например, «HVA», «ЗАФИКСИРОВАЛА).</span><span class="sxs-lookup"><span data-stu-id="c8583-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="c8583-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="c8583-158">vendorInformation</span></span> |[<span data-ttu-id="c8583-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="c8583-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="c8583-160">Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="c8583-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="c8583-161">**Поставщик и поставщика поля являются обязательными.**</span><span class="sxs-lookup"><span data-stu-id="c8583-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="c8583-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8583-162">Response</span></span>

<span data-ttu-id="c8583-163">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8583-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="c8583-164">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и объект обновленные [оповещения](../resources/alert.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c8583-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="c8583-165">Пример 1</span><span class="sxs-lookup"><span data-stu-id="c8583-165">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="c8583-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8583-166">Request</span></span>

<span data-ttu-id="c8583-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8583-167">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8583-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8583-168">Response</span></span>

<span data-ttu-id="c8583-169">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="c8583-169">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="c8583-170">Пример 2</span><span class="sxs-lookup"><span data-stu-id="c8583-170">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="c8583-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8583-171">Request</span></span>

<span data-ttu-id="c8583-172">В следующем примере показан запрос, который включает в себя `Prefer` заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="c8583-172">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="c8583-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8583-173">Response</span></span>

<span data-ttu-id="c8583-174">Ниже приведен пример ответа при Дополнительно `Prefer: return=representation` используется заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="c8583-174">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="c8583-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8583-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
