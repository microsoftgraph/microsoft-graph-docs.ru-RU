---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c74babfb9f1a7e5cb58e4c6b9b79b4999b8bebd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017359"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="3207d-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3207d-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="3207d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3207d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3207d-105">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3207d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3207d-106">Prerequisites</span></span>
<span data-ttu-id="3207d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3207d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3207d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3207d-109">Permission type</span></span>|<span data-ttu-id="3207d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3207d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3207d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3207d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3207d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3207d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3207d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3207d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3207d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3207d-114">Not supported.</span></span>|
|<span data-ttu-id="3207d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3207d-115">Application</span></span>|<span data-ttu-id="3207d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3207d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3207d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3207d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3207d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3207d-118">Request headers</span></span>
|<span data-ttu-id="3207d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3207d-119">Header</span></span>|<span data-ttu-id="3207d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3207d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3207d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3207d-121">Authorization</span></span>|<span data-ttu-id="3207d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3207d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3207d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3207d-123">Accept</span></span>|<span data-ttu-id="3207d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3207d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3207d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3207d-125">Request body</span></span>
<span data-ttu-id="3207d-126">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3207d-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="3207d-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="3207d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3207d-128">Property</span></span>|<span data-ttu-id="3207d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3207d-129">Type</span></span>|<span data-ttu-id="3207d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3207d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3207d-131">id</span><span class="sxs-lookup"><span data-stu-id="3207d-131">id</span></span>|<span data-ttu-id="3207d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3207d-132">String</span></span>|<span data-ttu-id="3207d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3207d-133">Key of the entity.</span></span> <span data-ttu-id="3207d-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3207d-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3207d-135">createdDateTime</span></span>|<span data-ttu-id="3207d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3207d-136">DateTimeOffset</span></span>|<span data-ttu-id="3207d-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3207d-137">DateTime the object was created.</span></span> <span data-ttu-id="3207d-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3207d-139">description</span><span class="sxs-lookup"><span data-stu-id="3207d-139">description</span></span>|<span data-ttu-id="3207d-140">String</span><span class="sxs-lookup"><span data-stu-id="3207d-140">String</span></span>|<span data-ttu-id="3207d-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3207d-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3207d-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3207d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3207d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3207d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3207d-144">DateTimeOffset</span></span>|<span data-ttu-id="3207d-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3207d-145">DateTime the object was last modified.</span></span> <span data-ttu-id="3207d-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3207d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3207d-147">displayName</span></span>|<span data-ttu-id="3207d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="3207d-148">String</span></span>|<span data-ttu-id="3207d-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3207d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3207d-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3207d-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3207d-151">version</span><span class="sxs-lookup"><span data-stu-id="3207d-151">version</span></span>|<span data-ttu-id="3207d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3207d-152">Int32</span></span>|<span data-ttu-id="3207d-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3207d-153">Version of the device configuration.</span></span> <span data-ttu-id="3207d-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3207d-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3207d-155">passcodeBlockSimple</span></span>|<span data-ttu-id="3207d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="3207d-156">Boolean</span></span>|<span data-ttu-id="3207d-157">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="3207d-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="3207d-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3207d-158">passcodeExpirationDays</span></span>|<span data-ttu-id="3207d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3207d-159">Int32</span></span>|<span data-ttu-id="3207d-160">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="3207d-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="3207d-161">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="3207d-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="3207d-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3207d-162">passcodeMinimumLength</span></span>|<span data-ttu-id="3207d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3207d-163">Int32</span></span>|<span data-ttu-id="3207d-164">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="3207d-164">Minimum length of passcode.</span></span> <span data-ttu-id="3207d-165">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="3207d-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="3207d-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3207d-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3207d-167">Int32</span><span class="sxs-lookup"><span data-stu-id="3207d-167">Int32</span></span>|<span data-ttu-id="3207d-168">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="3207d-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="3207d-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="3207d-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="3207d-170">Int32</span><span class="sxs-lookup"><span data-stu-id="3207d-170">Int32</span></span>|<span data-ttu-id="3207d-171">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="3207d-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="3207d-172">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="3207d-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3207d-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3207d-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="3207d-174">Int32</span><span class="sxs-lookup"><span data-stu-id="3207d-174">Int32</span></span>|<span data-ttu-id="3207d-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="3207d-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3207d-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="3207d-176">passcodeRequiredType</span></span>|[<span data-ttu-id="3207d-177">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="3207d-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3207d-178">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="3207d-178">The required passcode type.</span></span> <span data-ttu-id="3207d-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3207d-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3207d-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="3207d-180">passcodeRequired</span></span>|<span data-ttu-id="3207d-181">Логический</span><span class="sxs-lookup"><span data-stu-id="3207d-181">Boolean</span></span>|<span data-ttu-id="3207d-182">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="3207d-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="3207d-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3207d-183">osMinimumVersion</span></span>|<span data-ttu-id="3207d-184">String</span><span class="sxs-lookup"><span data-stu-id="3207d-184">String</span></span>|<span data-ttu-id="3207d-185">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="3207d-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="3207d-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3207d-186">osMaximumVersion</span></span>|<span data-ttu-id="3207d-187">String</span><span class="sxs-lookup"><span data-stu-id="3207d-187">String</span></span>|<span data-ttu-id="3207d-188">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="3207d-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="3207d-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="3207d-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="3207d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3207d-190">Boolean</span></span>|<span data-ttu-id="3207d-191">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="3207d-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="3207d-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3207d-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3207d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="3207d-193">Boolean</span></span>|<span data-ttu-id="3207d-194">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="3207d-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="3207d-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3207d-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3207d-196">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="3207d-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3207d-197">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="3207d-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3207d-198">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3207d-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3207d-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="3207d-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="3207d-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="3207d-200">Boolean</span></span>|<span data-ttu-id="3207d-201">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3207d-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="3207d-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="3207d-202">Response</span></span>
<span data-ttu-id="3207d-203">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3207d-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3207d-204">Пример</span><span class="sxs-lookup"><span data-stu-id="3207d-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="3207d-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="3207d-205">Request</span></span>
<span data-ttu-id="3207d-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3207d-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="3207d-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="3207d-207">Response</span></span>
<span data-ttu-id="3207d-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3207d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



