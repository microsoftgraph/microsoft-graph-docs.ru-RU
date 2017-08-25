# <a name="update-organization"></a><span data-ttu-id="e5e5f-101">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="e5e5f-101">Update organization</span></span>

<span data-ttu-id="e5e5f-102">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-102">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5e5f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5e5f-103">Permissions</span></span>
<span data-ttu-id="e5e5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e5e5f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5e5f-106">Permission type</span></span>      | <span data-ttu-id="e5e5f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5e5f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e5e5f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5e5f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e5e5f-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-109">Not supported.</span></span>    | 
|<span data-ttu-id="e5e5f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5e5f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5e5f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-111">Not supported.</span></span>    | 
|<span data-ttu-id="e5e5f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5e5f-112">Application</span></span> | <span data-ttu-id="e5e5f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e5e5f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5e5f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="e5e5f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5e5f-115">Request headers</span></span>
| <span data-ttu-id="e5e5f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e5e5f-116">Name</span></span>       | <span data-ttu-id="e5e5f-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e5e5f-117">Type</span></span> | <span data-ttu-id="e5e5f-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e5e5f-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e5e5f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5e5f-119">Authorization</span></span>  | <span data-ttu-id="e5e5f-120">string</span><span class="sxs-lookup"><span data-stu-id="e5e5f-120">string</span></span>  | <span data-ttu-id="e5e5f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5e5f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5e5f-123">Request body</span></span>
<span data-ttu-id="e5e5f-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5e5f-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5e5f-127">Property</span></span>     | <span data-ttu-id="e5e5f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e5e5f-128">Type</span></span>   |<span data-ttu-id="e5e5f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e5e5f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5e5f-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="e5e5f-130">assignedPlans</span></span>|<span data-ttu-id="e5e5f-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="e5e5f-131">AssignedPlan</span></span>|<span data-ttu-id="e5e5f-p104">Коллекция планов обслуживания, сопоставленных с клиентом.                            **Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p104">The collection of service plans associated with the tenant.                            **Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5e5f-134">городу;</span><span class="sxs-lookup"><span data-stu-id="e5e5f-134">city</span></span>|<span data-ttu-id="e5e5f-135">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-135">String</span></span>|            |
|<span data-ttu-id="e5e5f-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="e5e5f-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="e5e5f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e5f-137">DateTimeOffset</span></span>|<span data-ttu-id="e5e5f-138">Время и дата последней синхронизации клиента с локальным каталогом.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="e5e5f-139">country</span><span class="sxs-lookup"><span data-stu-id="e5e5f-139">country</span></span>|<span data-ttu-id="e5e5f-140">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-140">String</span></span>|            |
|<span data-ttu-id="e5e5f-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="e5e5f-141">countryLetterCode</span></span>|<span data-ttu-id="e5e5f-142">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-142">String</span></span>|            |
|<span data-ttu-id="e5e5f-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="e5e5f-143">deletionTimestamp</span></span>|<span data-ttu-id="e5e5f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e5f-144">DateTimeOffset</span></span>||
|<span data-ttu-id="e5e5f-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="e5e5f-145">dirSyncEnabled</span></span>|<span data-ttu-id="e5e5f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5e5f-146">Boolean</span></span>|<span data-ttu-id="e5e5f-147">Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="e5e5f-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="e5e5f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e5e5f-148">displayName</span></span>|<span data-ttu-id="e5e5f-149">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-149">String</span></span>|<span data-ttu-id="e5e5f-150">Отображаемое имя для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="e5e5f-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="e5e5f-151">marketingNotificationEmails</span></span>|<span data-ttu-id="e5e5f-152">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-152">String</span></span>|                                        <span data-ttu-id="e5e5f-153">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5e5f-154">objectType</span><span class="sxs-lookup"><span data-stu-id="e5e5f-154">objectType</span></span>|<span data-ttu-id="e5e5f-155">Строка</span><span class="sxs-lookup"><span data-stu-id="e5e5f-155">String</span></span>|<span data-ttu-id="e5e5f-p105">Строка, которая определяет тип объекта. Для клиентов всегда задается значение Company. Наследуется от [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p105">A string that identifies the object type. For tenants the value is always “Company”. Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="e5e5f-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="e5e5f-159">postalCode</span></span>|<span data-ttu-id="e5e5f-160">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-160">String</span></span>|            |
|<span data-ttu-id="e5e5f-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="e5e5f-161">preferredLanguage</span></span>|<span data-ttu-id="e5e5f-162">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-162">String</span></span>|            |
|<span data-ttu-id="e5e5f-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="e5e5f-163">provisionedPlans</span></span>|<span data-ttu-id="e5e5f-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="e5e5f-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="e5e5f-165">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5e5f-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="e5e5f-166">provisioningErrors</span></span>|<span data-ttu-id="e5e5f-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="e5e5f-167">ProvisioningError</span></span>|                                        <span data-ttu-id="e5e5f-168">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5e5f-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="e5e5f-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="e5e5f-170">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-170">String</span></span>||
|<span data-ttu-id="e5e5f-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="e5e5f-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="e5e5f-172">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-172">String</span></span>||
|<span data-ttu-id="e5e5f-173">state</span><span class="sxs-lookup"><span data-stu-id="e5e5f-173">state</span></span>|<span data-ttu-id="e5e5f-174">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-174">String</span></span>|            |
|<span data-ttu-id="e5e5f-175">street</span><span class="sxs-lookup"><span data-stu-id="e5e5f-175">street</span></span>|<span data-ttu-id="e5e5f-176">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-176">String</span></span>|            |
|<span data-ttu-id="e5e5f-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="e5e5f-177">technicalNotificationMails</span></span>|<span data-ttu-id="e5e5f-178">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-178">String</span></span>|                                        <span data-ttu-id="e5e5f-179">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5e5f-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="e5e5f-180">telephoneNumber</span></span>|<span data-ttu-id="e5e5f-181">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-181">String</span></span>|            |
|<span data-ttu-id="e5e5f-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="e5e5f-182">verifiedDomains</span></span>|<span data-ttu-id="e5e5f-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="e5e5f-183">VerifiedDomain</span></span>|<span data-ttu-id="e5e5f-p106">Коллекция доменов, сопоставленных с этим клиентом.                            **Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p106">The collection of domains associated with this tenant.                            **Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="e5e5f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5e5f-186">Response</span></span>

<span data-ttu-id="e5e5f-187">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [organization](../resources/organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5e5f-188">Пример</span><span class="sxs-lookup"><span data-stu-id="e5e5f-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5e5f-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5e5f-189">Request</span></span>
<span data-ttu-id="e5e5f-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-190">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e5e5f-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5e5f-191">Response</span></span>
<span data-ttu-id="e5e5f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
