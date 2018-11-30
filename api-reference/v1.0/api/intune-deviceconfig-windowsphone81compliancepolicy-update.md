---
title: Обновление объекта windowsPhone81CompliancePolicy
description: Обновление свойств объекта windowsPhone81CompliancePolicy.
ms.openlocfilehash: a022a6823af42e897b6ae6f68230c0e2ac7861e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024750"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="90ec2-103">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="90ec2-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="90ec2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="90ec2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90ec2-105">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-105">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90ec2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="90ec2-106">Prerequisites</span></span>
<span data-ttu-id="90ec2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ec2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90ec2-109">Permission type</span></span>|<span data-ttu-id="90ec2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90ec2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ec2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90ec2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90ec2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ec2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90ec2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90ec2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ec2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ec2-114">Not supported.</span></span>|
|<span data-ttu-id="90ec2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90ec2-115">Application</span></span>|<span data-ttu-id="90ec2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ec2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ec2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90ec2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="90ec2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90ec2-118">Request headers</span></span>
|<span data-ttu-id="90ec2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90ec2-119">Header</span></span>|<span data-ttu-id="90ec2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="90ec2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ec2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90ec2-121">Authorization</span></span>|<span data-ttu-id="90ec2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="90ec2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ec2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="90ec2-123">Accept</span></span>|<span data-ttu-id="90ec2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90ec2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ec2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90ec2-125">Request body</span></span>
<span data-ttu-id="90ec2-126">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90ec2-126">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="90ec2-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-127">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="90ec2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ec2-128">Property</span></span>|<span data-ttu-id="90ec2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="90ec2-129">Type</span></span>|<span data-ttu-id="90ec2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="90ec2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ec2-131">id</span><span class="sxs-lookup"><span data-stu-id="90ec2-131">id</span></span>|<span data-ttu-id="90ec2-132">String</span><span class="sxs-lookup"><span data-stu-id="90ec2-132">String</span></span>|<span data-ttu-id="90ec2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90ec2-133">Key of the entity.</span></span> <span data-ttu-id="90ec2-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90ec2-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90ec2-135">createdDateTime</span></span>|<span data-ttu-id="90ec2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ec2-136">DateTimeOffset</span></span>|<span data-ttu-id="90ec2-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="90ec2-137">DateTime the object was created.</span></span> <span data-ttu-id="90ec2-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90ec2-139">описание</span><span class="sxs-lookup"><span data-stu-id="90ec2-139">description</span></span>|<span data-ttu-id="90ec2-140">String</span><span class="sxs-lookup"><span data-stu-id="90ec2-140">String</span></span>|<span data-ttu-id="90ec2-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90ec2-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90ec2-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90ec2-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90ec2-143">lastModifiedDateTime</span></span>|<span data-ttu-id="90ec2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ec2-144">DateTimeOffset</span></span>|<span data-ttu-id="90ec2-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="90ec2-145">DateTime the object was last modified.</span></span> <span data-ttu-id="90ec2-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90ec2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="90ec2-147">displayName</span></span>|<span data-ttu-id="90ec2-148">String</span><span class="sxs-lookup"><span data-stu-id="90ec2-148">String</span></span>|<span data-ttu-id="90ec2-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90ec2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90ec2-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90ec2-151">version</span><span class="sxs-lookup"><span data-stu-id="90ec2-151">version</span></span>|<span data-ttu-id="90ec2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="90ec2-152">Int32</span></span>|<span data-ttu-id="90ec2-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90ec2-153">Version of the device configuration.</span></span> <span data-ttu-id="90ec2-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="90ec2-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90ec2-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="90ec2-155">passwordBlockSimple</span></span>|<span data-ttu-id="90ec2-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="90ec2-156">Boolean</span></span>|<span data-ttu-id="90ec2-157">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="90ec2-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="90ec2-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="90ec2-158">passwordExpirationDays</span></span>|<span data-ttu-id="90ec2-159">Int32</span><span class="sxs-lookup"><span data-stu-id="90ec2-159">Int32</span></span>|<span data-ttu-id="90ec2-160">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="90ec2-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="90ec2-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="90ec2-161">passwordMinimumLength</span></span>|<span data-ttu-id="90ec2-162">Int32</span><span class="sxs-lookup"><span data-stu-id="90ec2-162">Int32</span></span>|<span data-ttu-id="90ec2-163">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="90ec2-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="90ec2-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="90ec2-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="90ec2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="90ec2-165">Int32</span></span>|<span data-ttu-id="90ec2-166">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="90ec2-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="90ec2-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="90ec2-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="90ec2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="90ec2-168">Int32</span></span>|<span data-ttu-id="90ec2-169">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="90ec2-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="90ec2-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="90ec2-170">passwordRequiredType</span></span>|[<span data-ttu-id="90ec2-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="90ec2-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="90ec2-172">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="90ec2-172">The required password type.</span></span> <span data-ttu-id="90ec2-173">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="90ec2-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="90ec2-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="90ec2-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="90ec2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="90ec2-175">Int32</span></span>|<span data-ttu-id="90ec2-176">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="90ec2-176">Number of previous passwords to block.</span></span> <span data-ttu-id="90ec2-177">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="90ec2-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="90ec2-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="90ec2-178">passwordRequired</span></span>|<span data-ttu-id="90ec2-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="90ec2-179">Boolean</span></span>|<span data-ttu-id="90ec2-180">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="90ec2-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="90ec2-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="90ec2-181">osMinimumVersion</span></span>|<span data-ttu-id="90ec2-182">String</span><span class="sxs-lookup"><span data-stu-id="90ec2-182">String</span></span>|<span data-ttu-id="90ec2-183">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="90ec2-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="90ec2-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="90ec2-184">osMaximumVersion</span></span>|<span data-ttu-id="90ec2-185">String</span><span class="sxs-lookup"><span data-stu-id="90ec2-185">String</span></span>|<span data-ttu-id="90ec2-186">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="90ec2-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="90ec2-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="90ec2-187">storageRequireEncryption</span></span>|<span data-ttu-id="90ec2-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="90ec2-188">Boolean</span></span>|<span data-ttu-id="90ec2-189">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="90ec2-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="90ec2-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ec2-190">Response</span></span>
<span data-ttu-id="90ec2-191">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90ec2-191">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ec2-192">Пример</span><span class="sxs-lookup"><span data-stu-id="90ec2-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="90ec2-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="90ec2-193">Request</span></span>
<span data-ttu-id="90ec2-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90ec2-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="90ec2-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="90ec2-195">Response</span></span>
<span data-ttu-id="90ec2-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="90ec2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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



