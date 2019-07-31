---
title: Обновление объекта windowsPhone81CompliancePolicy
description: Обновление свойств объекта windowsPhone81CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfdbe969fdd3f12abaaebc1ebb2126ad9acaf087
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986710"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="95b91-103">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="95b91-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="95b91-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95b91-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95b91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b91-106">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95b91-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="95b91-107">Prerequisites</span></span>
<span data-ttu-id="95b91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95b91-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95b91-110">Permission type</span></span>|<span data-ttu-id="95b91-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95b91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b91-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95b91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95b91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95b91-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95b91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b91-115">Not supported.</span></span>|
|<span data-ttu-id="95b91-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95b91-116">Application</span></span>|<span data-ttu-id="95b91-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b91-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95b91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="95b91-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95b91-119">Request headers</span></span>
|<span data-ttu-id="95b91-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95b91-120">Header</span></span>|<span data-ttu-id="95b91-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95b91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95b91-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95b91-122">Authorization</span></span>|<span data-ttu-id="95b91-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95b91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95b91-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95b91-124">Accept</span></span>|<span data-ttu-id="95b91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95b91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b91-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95b91-126">Request body</span></span>
<span data-ttu-id="95b91-127">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95b91-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="95b91-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="95b91-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95b91-129">Property</span></span>|<span data-ttu-id="95b91-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95b91-130">Type</span></span>|<span data-ttu-id="95b91-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95b91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b91-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95b91-132">roleScopeTagIds</span></span>|<span data-ttu-id="95b91-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95b91-133">String collection</span></span>|<span data-ttu-id="95b91-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="95b91-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95b91-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-136">id</span><span class="sxs-lookup"><span data-stu-id="95b91-136">id</span></span>|<span data-ttu-id="95b91-137">Строка</span><span class="sxs-lookup"><span data-stu-id="95b91-137">String</span></span>|<span data-ttu-id="95b91-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95b91-138">Key of the entity.</span></span> <span data-ttu-id="95b91-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95b91-140">createdDateTime</span></span>|<span data-ttu-id="95b91-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b91-141">DateTimeOffset</span></span>|<span data-ttu-id="95b91-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="95b91-142">DateTime the object was created.</span></span> <span data-ttu-id="95b91-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-144">description</span><span class="sxs-lookup"><span data-stu-id="95b91-144">description</span></span>|<span data-ttu-id="95b91-145">String</span><span class="sxs-lookup"><span data-stu-id="95b91-145">String</span></span>|<span data-ttu-id="95b91-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="95b91-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95b91-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95b91-148">lastModifiedDateTime</span></span>|<span data-ttu-id="95b91-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b91-149">DateTimeOffset</span></span>|<span data-ttu-id="95b91-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="95b91-150">DateTime the object was last modified.</span></span> <span data-ttu-id="95b91-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-152">displayName</span><span class="sxs-lookup"><span data-stu-id="95b91-152">displayName</span></span>|<span data-ttu-id="95b91-153">Строка</span><span class="sxs-lookup"><span data-stu-id="95b91-153">String</span></span>|<span data-ttu-id="95b91-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="95b91-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95b91-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95b91-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-156">version</span><span class="sxs-lookup"><span data-stu-id="95b91-156">version</span></span>|<span data-ttu-id="95b91-157">Int32</span><span class="sxs-lookup"><span data-stu-id="95b91-157">Int32</span></span>|<span data-ttu-id="95b91-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="95b91-158">Version of the device configuration.</span></span> <span data-ttu-id="95b91-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95b91-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95b91-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="95b91-160">passwordBlockSimple</span></span>|<span data-ttu-id="95b91-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="95b91-161">Boolean</span></span>|<span data-ttu-id="95b91-162">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="95b91-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="95b91-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="95b91-163">passwordExpirationDays</span></span>|<span data-ttu-id="95b91-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95b91-164">Int32</span></span>|<span data-ttu-id="95b91-165">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="95b91-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="95b91-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="95b91-166">passwordMinimumLength</span></span>|<span data-ttu-id="95b91-167">Int32</span><span class="sxs-lookup"><span data-stu-id="95b91-167">Int32</span></span>|<span data-ttu-id="95b91-168">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="95b91-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="95b91-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="95b91-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="95b91-170">Int32</span><span class="sxs-lookup"><span data-stu-id="95b91-170">Int32</span></span>|<span data-ttu-id="95b91-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="95b91-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="95b91-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="95b91-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="95b91-173">Int32</span><span class="sxs-lookup"><span data-stu-id="95b91-173">Int32</span></span>|<span data-ttu-id="95b91-174">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="95b91-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="95b91-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="95b91-175">passwordRequiredType</span></span>|[<span data-ttu-id="95b91-176">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="95b91-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="95b91-177">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="95b91-177">The required password type.</span></span> <span data-ttu-id="95b91-178">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="95b91-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="95b91-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="95b91-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="95b91-180">Int32</span><span class="sxs-lookup"><span data-stu-id="95b91-180">Int32</span></span>|<span data-ttu-id="95b91-181">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="95b91-181">Number of previous passwords to block.</span></span> <span data-ttu-id="95b91-182">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="95b91-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="95b91-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="95b91-183">passwordRequired</span></span>|<span data-ttu-id="95b91-184">Логический</span><span class="sxs-lookup"><span data-stu-id="95b91-184">Boolean</span></span>|<span data-ttu-id="95b91-185">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="95b91-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="95b91-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="95b91-186">osMinimumVersion</span></span>|<span data-ttu-id="95b91-187">String</span><span class="sxs-lookup"><span data-stu-id="95b91-187">String</span></span>|<span data-ttu-id="95b91-188">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="95b91-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="95b91-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="95b91-189">osMaximumVersion</span></span>|<span data-ttu-id="95b91-190">String</span><span class="sxs-lookup"><span data-stu-id="95b91-190">String</span></span>|<span data-ttu-id="95b91-191">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="95b91-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="95b91-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="95b91-192">storageRequireEncryption</span></span>|<span data-ttu-id="95b91-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="95b91-193">Boolean</span></span>|<span data-ttu-id="95b91-194">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="95b91-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="95b91-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="95b91-195">Response</span></span>
<span data-ttu-id="95b91-196">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95b91-196">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95b91-197">Пример</span><span class="sxs-lookup"><span data-stu-id="95b91-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="95b91-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="95b91-198">Request</span></span>
<span data-ttu-id="95b91-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95b91-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="95b91-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="95b91-200">Response</span></span>
<span data-ttu-id="95b91-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95b91-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





