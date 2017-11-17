# <a name="update-organization"></a><span data-ttu-id="39be7-101">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="39be7-101">Update organization</span></span>

<span data-ttu-id="39be7-102">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="39be7-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="39be7-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39be7-103">Permissions</span></span>

<span data-ttu-id="39be7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="39be7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39be7-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39be7-106">Permission type</span></span>      | <span data-ttu-id="39be7-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39be7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39be7-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39be7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="39be7-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39be7-109">Not supported.</span></span>    |
|<span data-ttu-id="39be7-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39be7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39be7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39be7-111">Not supported.</span></span>    |
|<span data-ttu-id="39be7-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39be7-112">Application</span></span> | <span data-ttu-id="39be7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39be7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39be7-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39be7-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="39be7-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39be7-115">Request headers</span></span>

| <span data-ttu-id="39be7-116">Имя</span><span class="sxs-lookup"><span data-stu-id="39be7-116">Name</span></span>       | <span data-ttu-id="39be7-117">Тип</span><span class="sxs-lookup"><span data-stu-id="39be7-117">Type</span></span> | <span data-ttu-id="39be7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="39be7-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="39be7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="39be7-119">Authorization</span></span>  | <span data-ttu-id="39be7-120">string</span><span class="sxs-lookup"><span data-stu-id="39be7-120">string</span></span>  | <span data-ttu-id="39be7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39be7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39be7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39be7-123">Request body</span></span>
<span data-ttu-id="39be7-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="39be7-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="39be7-125">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="39be7-125">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="39be7-126">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="39be7-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="39be7-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="39be7-127">Property</span></span>     | <span data-ttu-id="39be7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="39be7-128">Type</span></span>   |<span data-ttu-id="39be7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="39be7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39be7-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="39be7-130">assignedPlans</span></span>|<span data-ttu-id="39be7-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="39be7-131">AssignedPlan</span></span>|<span data-ttu-id="39be7-132">Коллекция планов обслуживания, сопоставленных с клиентом.</span><span class="sxs-lookup"><span data-stu-id="39be7-132">The collection of service plans associated with the tenant. Not nullable.</span></span> <span data-ttu-id="39be7-133">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="39be7-133">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="39be7-134">city</span><span class="sxs-lookup"><span data-stu-id="39be7-134">city</span></span>|<span data-ttu-id="39be7-135">String</span><span class="sxs-lookup"><span data-stu-id="39be7-135">String</span></span>|            |
|<span data-ttu-id="39be7-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="39be7-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="39be7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39be7-137">DateTimeOffset</span></span>|<span data-ttu-id="39be7-138">Время и дата последней синхронизации клиента с локальным каталогом.</span><span class="sxs-lookup"><span data-stu-id="39be7-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="39be7-139">country</span><span class="sxs-lookup"><span data-stu-id="39be7-139">country</span></span>|<span data-ttu-id="39be7-140">String</span><span class="sxs-lookup"><span data-stu-id="39be7-140">String</span></span>|            |
|<span data-ttu-id="39be7-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="39be7-141">countryLetterCode</span></span>|<span data-ttu-id="39be7-142">String</span><span class="sxs-lookup"><span data-stu-id="39be7-142">String</span></span>|            |
|<span data-ttu-id="39be7-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="39be7-143">deletionTimestamp</span></span>|<span data-ttu-id="39be7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39be7-144">DateTimeOffset</span></span>||
|<span data-ttu-id="39be7-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="39be7-145">dirSyncEnabled</span></span>|<span data-ttu-id="39be7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="39be7-146">Boolean</span></span>|<span data-ttu-id="39be7-147">Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="39be7-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="39be7-148">displayName</span><span class="sxs-lookup"><span data-stu-id="39be7-148">displayName</span></span>|<span data-ttu-id="39be7-149">String</span><span class="sxs-lookup"><span data-stu-id="39be7-149">String</span></span>|<span data-ttu-id="39be7-150">Отображаемое имя для клиента.</span><span class="sxs-lookup"><span data-stu-id="39be7-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="39be7-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="39be7-151">marketingNotificationEmails</span></span>|<span data-ttu-id="39be7-152">String</span><span class="sxs-lookup"><span data-stu-id="39be7-152">String</span></span>|                                        <span data-ttu-id="39be7-153">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="39be7-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="39be7-154">objectType</span><span class="sxs-lookup"><span data-stu-id="39be7-154">objectType</span></span>|<span data-ttu-id="39be7-155">String</span><span class="sxs-lookup"><span data-stu-id="39be7-155">String</span></span>|<span data-ttu-id="39be7-156">Строка, которая определяет тип объекта.</span><span class="sxs-lookup"><span data-stu-id="39be7-156">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="39be7-157">Для клиентов всегда задается значение Company.</span><span class="sxs-lookup"><span data-stu-id="39be7-157">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="39be7-158">Наследуется от [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="39be7-158">Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="39be7-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="39be7-159">postalCode</span></span>|<span data-ttu-id="39be7-160">String</span><span class="sxs-lookup"><span data-stu-id="39be7-160">String</span></span>|            |
|<span data-ttu-id="39be7-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="39be7-161">preferredLanguage</span></span>|<span data-ttu-id="39be7-162">String</span><span class="sxs-lookup"><span data-stu-id="39be7-162">String</span></span>|            |
|<span data-ttu-id="39be7-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="39be7-163">provisionedPlans</span></span>|<span data-ttu-id="39be7-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="39be7-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="39be7-165">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="39be7-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="39be7-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="39be7-166">provisioningErrors</span></span>|<span data-ttu-id="39be7-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="39be7-167">ProvisioningError</span></span>|                                        <span data-ttu-id="39be7-168">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="39be7-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="39be7-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="39be7-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="39be7-170">String</span><span class="sxs-lookup"><span data-stu-id="39be7-170">String</span></span>||
|<span data-ttu-id="39be7-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="39be7-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="39be7-172">String</span><span class="sxs-lookup"><span data-stu-id="39be7-172">String</span></span>||
|<span data-ttu-id="39be7-173">state</span><span class="sxs-lookup"><span data-stu-id="39be7-173">state</span></span>|<span data-ttu-id="39be7-174">String</span><span class="sxs-lookup"><span data-stu-id="39be7-174">String</span></span>|            |
|<span data-ttu-id="39be7-175">street</span><span class="sxs-lookup"><span data-stu-id="39be7-175">street</span></span>|<span data-ttu-id="39be7-176">String</span><span class="sxs-lookup"><span data-stu-id="39be7-176">String</span></span>|            |
|<span data-ttu-id="39be7-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="39be7-177">technicalNotificationMails</span></span>|<span data-ttu-id="39be7-178">String</span><span class="sxs-lookup"><span data-stu-id="39be7-178">String</span></span>|                                        <span data-ttu-id="39be7-179">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="39be7-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="39be7-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="39be7-180">telephoneNumber</span></span>|<span data-ttu-id="39be7-181">String</span><span class="sxs-lookup"><span data-stu-id="39be7-181">String</span></span>|            |
|<span data-ttu-id="39be7-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="39be7-182">verifiedDomains</span></span>|<span data-ttu-id="39be7-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="39be7-183">VerifiedDomain</span></span>|<span data-ttu-id="39be7-184">Коллекция доменов, сопоставленных с этим клиентом.</span><span class="sxs-lookup"><span data-stu-id="39be7-184">The collection of domains associated with this tenant. Not nullable.</span></span> <span data-ttu-id="39be7-185">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="39be7-185">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="39be7-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="39be7-186">Response</span></span>

<span data-ttu-id="39be7-187">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [organization](../resources/organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39be7-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39be7-188">Пример</span><span class="sxs-lookup"><span data-stu-id="39be7-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="39be7-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="39be7-189">Request</span></span>

<span data-ttu-id="39be7-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39be7-190">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

### <a name="response"></a><span data-ttu-id="39be7-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="39be7-191">Response</span></span>

<span data-ttu-id="39be7-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39be7-192">Here is an example of the response.</span></span> <span data-ttu-id="39be7-193">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="39be7-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="39be7-194">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39be7-194">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
