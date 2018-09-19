# <a name="update-alert"></a><span data-ttu-id="91674-101">Оповещение обновления</span><span class="sxs-lookup"><span data-stu-id="91674-101">Update alert</span></span>

<span data-ttu-id="91674-102">Обновите редактируемое свойство **оповещения** в любом интегрированном решении для синхронизации состояний оповещений и назначений в синхронизации решений.</span><span class="sxs-lookup"><span data-stu-id="91674-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="91674-103">Этот метод обновляет все решения, у которых есть запись идентификатора указанного оповещения.</span><span class="sxs-lookup"><span data-stu-id="91674-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="91674-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91674-104">Permissions</span></span>

<span data-ttu-id="91674-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91674-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91674-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91674-107">Permission type</span></span>      | <span data-ttu-id="91674-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91674-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91674-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91674-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="91674-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91674-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="91674-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91674-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91674-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91674-112">Not supported.</span></span>  |
|<span data-ttu-id="91674-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91674-113">Application</span></span> | <span data-ttu-id="91674-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91674-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91674-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91674-115">HTTP request</span></span>

> <span data-ttu-id="91674-116">**Примечание:** с этим методом необходимо указать идентификатор **оповещения** в качестве параметра и информацию о производителе, содержащую `provider` и `vendor`.</span><span class="sxs-lookup"><span data-stu-id="91674-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="91674-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91674-117">Request headers</span></span>

| <span data-ttu-id="91674-118">Имя</span><span class="sxs-lookup"><span data-stu-id="91674-118">Name</span></span>       | <span data-ttu-id="91674-119">Описание</span><span class="sxs-lookup"><span data-stu-id="91674-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="91674-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91674-120">Authorization</span></span>  | <span data-ttu-id="91674-p103">"Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91674-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="91674-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="91674-123">Prefer</span></span> | <span data-ttu-id="91674-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="91674-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="91674-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91674-125">Request body</span></span>

<span data-ttu-id="91674-126">В тексте запроса укажите представление JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="91674-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="91674-127">Текст **должен** содержать `vendorInformation` свойство с допустимыми полями `provider` и `vendor`.</span><span class="sxs-lookup"><span data-stu-id="91674-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="91674-128">В следующей таблице приведены поля, которые могут быть обновлены для оповещения.</span><span class="sxs-lookup"><span data-stu-id="91674-128">The following table lists the authentication settings that can be changed for an authentication provider.</span></span> <span data-ttu-id="91674-129">Значения для существующих свойств, которые не включены в текст запроса, остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="91674-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="91674-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="91674-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91674-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="91674-131">Property</span></span>   | <span data-ttu-id="91674-132">Тип</span><span class="sxs-lookup"><span data-stu-id="91674-132">Type</span></span> |<span data-ttu-id="91674-133">Описание</span><span class="sxs-lookup"><span data-stu-id="91674-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91674-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="91674-134">assignedTo</span></span>|<span data-ttu-id="91674-135">String</span><span class="sxs-lookup"><span data-stu-id="91674-135">String</span></span>|<span data-ttu-id="91674-136">Имя аналитики, которой назначено оповещение для рассмотрения, исследования и исправления.</span><span class="sxs-lookup"><span data-stu-id="91674-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="91674-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="91674-137">closedDateTime</span></span>|<span data-ttu-id="91674-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91674-138">DateTimeOffset</span></span>|<span data-ttu-id="91674-139">Дата и время закрытия оповещения.</span><span class="sxs-lookup"><span data-stu-id="91674-139">Time at which the alert was closed.</span></span> <span data-ttu-id="91674-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="91674-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="91674-141">Например, значение для полуночи 1 января 2014 года в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="91674-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="91674-142">comments</span><span class="sxs-lookup"><span data-stu-id="91674-142">comments</span></span>|<span data-ttu-id="91674-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91674-143">String collection</span></span>|<span data-ttu-id="91674-144">Комментарии аналитика по оповещению (для управления предупреждениями клиента).</span><span class="sxs-lookup"><span data-stu-id="91674-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="91674-145">feedback</span><span class="sxs-lookup"><span data-stu-id="91674-145">Feedback</span></span>|<span data-ttu-id="91674-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="91674-146">alertFeedback</span></span>|<span data-ttu-id="91674-147">Отчет аналитика относительно оповещения.</span><span class="sxs-lookup"><span data-stu-id="91674-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="91674-148">Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="91674-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="91674-149">status</span><span class="sxs-lookup"><span data-stu-id="91674-149">status</span></span>|<span data-ttu-id="91674-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="91674-150">alertStatus</span></span>|<span data-ttu-id="91674-151">Статус жизненного цикла оповещения (стадия).</span><span class="sxs-lookup"><span data-stu-id="91674-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="91674-152">Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="91674-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="91674-153">tags</span><span class="sxs-lookup"><span data-stu-id="91674-153">Tags</span></span>|<span data-ttu-id="91674-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91674-154">String collection</span></span>|<span data-ttu-id="91674-155">Определяемые пользователем метки, которые могут применяться к оповещению и выступать в качестве условий фильтра (например, "HVA", "SAW").</span><span class="sxs-lookup"><span data-stu-id="91674-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="91674-156">vendorInformation \*</span><span class="sxs-lookup"><span data-stu-id="91674-156">vendorInformation \*</span></span>|[<span data-ttu-id="91674-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="91674-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="91674-158">Комплексный тип, в котором содержатся сведения о безопасности продуктов и услуг разработчика, поставщика и субпоставщика (например, производитель = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="91674-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="91674-159">**Поля поставщика и производителя являются обязательными.**</span><span class="sxs-lookup"><span data-stu-id="91674-159">**Provider and vendor fields are required.**</span></span>|
<span data-ttu-id="91674-160">(\* Указывает на обязательное поле.)</span><span class="sxs-lookup"><span data-stu-id="91674-160">(\* Indicates a mandatory field.)</span></span>

## <a name="response"></a><span data-ttu-id="91674-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="91674-161">Response</span></span>

<span data-ttu-id="91674-162">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91674-162">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="91674-163">Если используется запрос на необязательный заголовок, метод возвращает код отклика `200 OK` и обновленный объект [оповещения](../resources/alert.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91674-163">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="91674-164">Пример 1</span><span class="sxs-lookup"><span data-stu-id="91674-164">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="91674-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="91674-165">Request</span></span>

<span data-ttu-id="91674-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91674-166">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91674-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="91674-167">Response</span></span>

<span data-ttu-id="91674-168">Ниже приведен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="91674-168">The following is an example of a response to a  event.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="91674-169">Пример 2</span><span class="sxs-lookup"><span data-stu-id="91674-169">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="91674-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="91674-170">Request</span></span>

<span data-ttu-id="91674-171">В следующем примере показан запрос, который включает в себя заголовок запроса `Prefer`.</span><span class="sxs-lookup"><span data-stu-id="91674-171">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="91674-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="91674-172">Response</span></span>

<span data-ttu-id="91674-173">Ниже приведен пример отклика, в котором используется необязательный заголовок запроса `Prefer: return=representation`.</span><span class="sxs-lookup"><span data-stu-id="91674-173">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="91674-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91674-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
