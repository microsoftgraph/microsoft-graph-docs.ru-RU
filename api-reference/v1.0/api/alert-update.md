---
title: Обновление оповещения
description: Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях. Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 42bc945dde726466439802350796d628ee438e22
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967321"
---
# <a name="update-alert"></a><span data-ttu-id="d99b2-104">Обновление оповещения</span><span class="sxs-lookup"><span data-stu-id="d99b2-104">Update alert</span></span>

<span data-ttu-id="d99b2-105">Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.</span><span class="sxs-lookup"><span data-stu-id="d99b2-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="d99b2-106">Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d99b2-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d99b2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d99b2-107">Permissions</span></span>

<span data-ttu-id="d99b2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d99b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d99b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d99b2-110">Permission type</span></span>                        | <span data-ttu-id="d99b2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d99b2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="d99b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d99b2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d99b2-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d99b2-113">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="d99b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d99b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d99b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d99b2-115">Not supported.</span></span>                      |
| <span data-ttu-id="d99b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d99b2-116">Application</span></span>                            | <span data-ttu-id="d99b2-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d99b2-117">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="d99b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d99b2-118">HTTP request</span></span>

> <span data-ttu-id="d99b2-119">**Примечание:** Необходимо указать код **оповещение о** как параметр и содержащий vendorInformation `provider` и `vendor` с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="d99b2-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="d99b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d99b2-120">Request headers</span></span>

| <span data-ttu-id="d99b2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d99b2-121">Name</span></span>          | <span data-ttu-id="d99b2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d99b2-122">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="d99b2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d99b2-123">Authorization</span></span> | <span data-ttu-id="d99b2-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d99b2-p104">Bearer {code}. Required.</span></span> |
| <span data-ttu-id="d99b2-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="d99b2-126">Prefer</span></span>        | <span data-ttu-id="d99b2-127">Возвращает = представление</span><span class="sxs-lookup"><span data-stu-id="d99b2-127">return=representation</span></span>    |

## <a name="request-body"></a><span data-ttu-id="d99b2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d99b2-128">Request body</span></span>

<span data-ttu-id="d99b2-129">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="d99b2-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d99b2-130">Текст, **должны** содержать `vendorInformation` свойство с допустимыми `provider` и `vendor` полей.</span><span class="sxs-lookup"><span data-stu-id="d99b2-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="d99b2-131">В следующей таблице приведены поля, которые могут быть обновлены для оповещения.</span><span class="sxs-lookup"><span data-stu-id="d99b2-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="d99b2-132">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="d99b2-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="d99b2-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d99b2-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d99b2-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d99b2-134">Property</span></span>          | <span data-ttu-id="d99b2-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d99b2-135">Type</span></span>                                                                   | <span data-ttu-id="d99b2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d99b2-136">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="d99b2-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d99b2-137">assignedTo</span></span>        | <span data-ttu-id="d99b2-138">String</span><span class="sxs-lookup"><span data-stu-id="d99b2-138">String</span></span>                                                                 | <span data-ttu-id="d99b2-139">Имя аналитик оповещение будет назначен для рассмотрения исследования и исправления.</span><span class="sxs-lookup"><span data-stu-id="d99b2-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="d99b2-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d99b2-140">closedDateTime</span></span>    | <span data-ttu-id="d99b2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d99b2-141">DateTimeOffset</span></span>                                                         | <span data-ttu-id="d99b2-142">Время закрытия оповещение.</span><span class="sxs-lookup"><span data-stu-id="d99b2-142">Time at which the alert was closed.</span></span> <span data-ttu-id="d99b2-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d99b2-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d99b2-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d99b2-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="d99b2-145">comments</span><span class="sxs-lookup"><span data-stu-id="d99b2-145">comments</span></span>          | <span data-ttu-id="d99b2-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d99b2-146">String collection</span></span>                                                      | <span data-ttu-id="d99b2-147">Комментарии аналитик оповещения (для управления предупреждениями клиента).</span><span class="sxs-lookup"><span data-stu-id="d99b2-147">Analyst comments on the alert (for customer alert management).</span></span> |
| <span data-ttu-id="d99b2-148">свои отзывы и предложения</span><span class="sxs-lookup"><span data-stu-id="d99b2-148">feedback</span></span>          | <span data-ttu-id="d99b2-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="d99b2-149">alertFeedback</span></span>                                                          | <span data-ttu-id="d99b2-150">Отзыв аналитик на оповещение.</span><span class="sxs-lookup"><span data-stu-id="d99b2-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="d99b2-151">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="d99b2-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="d99b2-152">status</span><span class="sxs-lookup"><span data-stu-id="d99b2-152">status</span></span>            | <span data-ttu-id="d99b2-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="d99b2-153">alertStatus</span></span>                                                            | <span data-ttu-id="d99b2-154">Состояние оповещений жизненного цикла (рабочей области).</span><span class="sxs-lookup"><span data-stu-id="d99b2-154">Alert life cycle status (stage).</span></span> <span data-ttu-id="d99b2-155">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="d99b2-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="d99b2-156">tags</span><span class="sxs-lookup"><span data-stu-id="d99b2-156">tags</span></span>              | <span data-ttu-id="d99b2-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d99b2-157">String collection</span></span>                                                      | <span data-ttu-id="d99b2-158">Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например, «HVA», «ЗАФИКСИРОВАЛА).</span><span class="sxs-lookup"><span data-stu-id="d99b2-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="d99b2-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="d99b2-159">vendorInformation</span></span> | [<span data-ttu-id="d99b2-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="d99b2-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="d99b2-161">Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="d99b2-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="d99b2-162">**Поставщик и поставщика поля являются обязательными.**</span><span class="sxs-lookup"><span data-stu-id="d99b2-162">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="d99b2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="d99b2-163">Response</span></span>

<span data-ttu-id="d99b2-164">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d99b2-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="d99b2-165">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и объект обновленные [оповещения](../resources/alert.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d99b2-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d99b2-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="d99b2-166">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="d99b2-167">В примере 1: Запрос без Prefer заголовка</span><span class="sxs-lookup"><span data-stu-id="d99b2-167">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="d99b2-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="d99b2-168">Request</span></span>

<span data-ttu-id="d99b2-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d99b2-169">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="d99b2-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d99b2-170">Response</span></span>

<span data-ttu-id="d99b2-171">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="d99b2-171">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="d99b2-172">Пример 2: Запрос с заголовком, Prefer</span><span class="sxs-lookup"><span data-stu-id="d99b2-172">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="d99b2-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="d99b2-173">Request</span></span>

<span data-ttu-id="d99b2-174">В следующем примере показан запрос, который включает в себя `Prefer` заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="d99b2-174">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d99b2-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="d99b2-175">Response</span></span>

<span data-ttu-id="d99b2-176">Ниже приведен пример ответа при Дополнительно `Prefer: return=representation` используется заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="d99b2-176">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="d99b2-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d99b2-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
