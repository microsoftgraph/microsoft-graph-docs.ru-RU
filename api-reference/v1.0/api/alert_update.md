# <a name="update-alert"></a><span data-ttu-id="73a12-101">обновление оповещения.</span><span class="sxs-lookup"><span data-stu-id="73a12-101">Update alert</span></span>

<span data-ttu-id="73a12-102">Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.</span><span class="sxs-lookup"><span data-stu-id="73a12-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="73a12-103">Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="73a12-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a12-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73a12-104">Permissions</span></span>

<span data-ttu-id="73a12-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73a12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73a12-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73a12-107">Permission type</span></span>      | <span data-ttu-id="73a12-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73a12-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73a12-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73a12-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="73a12-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73a12-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="73a12-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73a12-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="73a12-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73a12-112">Not supported.</span></span>  |
|<span data-ttu-id="73a12-113">Для приложения</span><span class="sxs-lookup"><span data-stu-id="73a12-113">Application</span></span> | <span data-ttu-id="73a12-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73a12-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73a12-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73a12-115">HTTP request</span></span>

> <span data-ttu-id="73a12-116">**Примечание:** Необходимо указать код **оповещение о** как параметр и содержащий vendorInformation `provider` и `vendor` с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="73a12-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="73a12-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73a12-117">Request headers</span></span>

| <span data-ttu-id="73a12-118">Имя</span><span class="sxs-lookup"><span data-stu-id="73a12-118">Name</span></span>       | <span data-ttu-id="73a12-119">Описание</span><span class="sxs-lookup"><span data-stu-id="73a12-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="73a12-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="73a12-120">Authorization</span></span>  | <span data-ttu-id="73a12-p103">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73a12-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="73a12-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="73a12-123">Prefer</span></span> | <span data-ttu-id="73a12-124">Возвращает = представление</span><span class="sxs-lookup"><span data-stu-id="73a12-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="73a12-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73a12-125">Request body</span></span>

<span data-ttu-id="73a12-126">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="73a12-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="73a12-127">Текст, **должны** содержать `vendorInformation` свойство с допустимыми `provider` и `vendor` полей.</span><span class="sxs-lookup"><span data-stu-id="73a12-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="73a12-128">В следующей таблице приведены поля, которые могут быть обновлены для оповещения.</span><span class="sxs-lookup"><span data-stu-id="73a12-128">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="73a12-129">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="73a12-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="73a12-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="73a12-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73a12-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="73a12-131">Property</span></span>   | <span data-ttu-id="73a12-132">Тип</span><span class="sxs-lookup"><span data-stu-id="73a12-132">Type</span></span> |<span data-ttu-id="73a12-133">Описание</span><span class="sxs-lookup"><span data-stu-id="73a12-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73a12-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="73a12-134">assignedTo</span></span>|<span data-ttu-id="73a12-135">String</span><span class="sxs-lookup"><span data-stu-id="73a12-135">String</span></span>|<span data-ttu-id="73a12-136">Имя аналитик оповещение будет назначен для рассмотрения исследования и исправления.</span><span class="sxs-lookup"><span data-stu-id="73a12-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="73a12-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="73a12-137">closedDateTime</span></span>|<span data-ttu-id="73a12-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73a12-138">DateTimeOffset</span></span>|<span data-ttu-id="73a12-139">Время закрытия оповещение.</span><span class="sxs-lookup"><span data-stu-id="73a12-139">Time at which the alert was closed.</span></span> <span data-ttu-id="73a12-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="73a12-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73a12-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="73a12-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="73a12-142">comments</span><span class="sxs-lookup"><span data-stu-id="73a12-142">comments</span></span>|<span data-ttu-id="73a12-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="73a12-143">String collection</span></span>|<span data-ttu-id="73a12-144">Комментарии аналитик оповещения (для управления предупреждениями клиента).</span><span class="sxs-lookup"><span data-stu-id="73a12-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="73a12-145">свои отзывы и предложения</span><span class="sxs-lookup"><span data-stu-id="73a12-145">feedback</span></span>|<span data-ttu-id="73a12-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="73a12-146">alertFeedback</span></span>|<span data-ttu-id="73a12-147">Отзыв аналитик на оповещение.</span><span class="sxs-lookup"><span data-stu-id="73a12-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="73a12-148">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="73a12-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="73a12-149">status</span><span class="sxs-lookup"><span data-stu-id="73a12-149">status</span></span>|<span data-ttu-id="73a12-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="73a12-150">alertStatus</span></span>|<span data-ttu-id="73a12-151">Состояние оповещений жизненного цикла (рабочей области).</span><span class="sxs-lookup"><span data-stu-id="73a12-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="73a12-152">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="73a12-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="73a12-153">теги</span><span class="sxs-lookup"><span data-stu-id="73a12-153">tags</span></span>|<span data-ttu-id="73a12-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="73a12-154">String collection</span></span>|<span data-ttu-id="73a12-155">Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например, «HVA», «ЗАФИКСИРОВАЛА).</span><span class="sxs-lookup"><span data-stu-id="73a12-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="73a12-156">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="73a12-156">vendorInformation</span></span> |[<span data-ttu-id="73a12-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="73a12-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="73a12-158">Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="73a12-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="73a12-159">**Поставщик и поставщика поля являются обязательными.**</span><span class="sxs-lookup"><span data-stu-id="73a12-159">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="73a12-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="73a12-160">Response</span></span>

<span data-ttu-id="73a12-161">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="73a12-161">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="73a12-162">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и объект обновленные [оповещения](../resources/alert.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73a12-162">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="73a12-163">Пример 1</span><span class="sxs-lookup"><span data-stu-id="73a12-163">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="73a12-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="73a12-164">Request</span></span>

<span data-ttu-id="73a12-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73a12-165">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73a12-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="73a12-166">Response</span></span>

<span data-ttu-id="73a12-167">Ниже приведен пример успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="73a12-167">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="73a12-168">Пример 2</span><span class="sxs-lookup"><span data-stu-id="73a12-168">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="73a12-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="73a12-169">Request</span></span>

<span data-ttu-id="73a12-170">В следующем примере показан запрос, который включает в себя `Prefer` заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="73a12-170">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="73a12-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="73a12-171">Response</span></span>

<span data-ttu-id="73a12-172">Ниже приведен пример ответа при Дополнительно `Prefer: return=representation` используется заголовка запроса.</span><span class="sxs-lookup"><span data-stu-id="73a12-172">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="73a12-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73a12-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
