---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62fd1d293823c07b35125e688d8b6a3235fc8d02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972961"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="1f329-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1f329-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="1f329-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f329-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f329-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f329-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f329-106">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f329-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f329-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1f329-107">Prerequisites</span></span>
<span data-ttu-id="1f329-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f329-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f329-110">Permission type</span></span>|<span data-ttu-id="1f329-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f329-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f329-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f329-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f329-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f329-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f329-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f329-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f329-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f329-115">Not supported.</span></span>|
|<span data-ttu-id="1f329-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f329-116">Application</span></span>|<span data-ttu-id="1f329-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f329-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f329-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f329-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1f329-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f329-119">Request headers</span></span>
|<span data-ttu-id="1f329-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f329-120">Header</span></span>|<span data-ttu-id="1f329-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1f329-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f329-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f329-122">Authorization</span></span>|<span data-ttu-id="1f329-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f329-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f329-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1f329-124">Accept</span></span>|<span data-ttu-id="1f329-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f329-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f329-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f329-126">Request body</span></span>
<span data-ttu-id="1f329-127">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f329-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="1f329-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="1f329-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="1f329-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f329-129">Property</span></span>|<span data-ttu-id="1f329-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1f329-130">Type</span></span>|<span data-ttu-id="1f329-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1f329-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f329-132">description</span><span class="sxs-lookup"><span data-stu-id="1f329-132">description</span></span>|<span data-ttu-id="1f329-133">String</span><span class="sxs-lookup"><span data-stu-id="1f329-133">String</span></span>|<span data-ttu-id="1f329-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f329-134">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f329-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f329-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f329-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1f329-136">displayName</span></span>|<span data-ttu-id="1f329-137">String</span><span class="sxs-lookup"><span data-stu-id="1f329-137">String</span></span>|<span data-ttu-id="1f329-138">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f329-138">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f329-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f329-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f329-140">version</span><span class="sxs-lookup"><span data-stu-id="1f329-140">version</span></span>|<span data-ttu-id="1f329-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1f329-141">Int32</span></span>|<span data-ttu-id="1f329-142">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f329-142">Version of the device configuration.</span></span> <span data-ttu-id="1f329-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f329-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f329-144">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1f329-144">passcodeBlockSimple</span></span>|<span data-ttu-id="1f329-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f329-145">Boolean</span></span>|<span data-ttu-id="1f329-146">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="1f329-146">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="1f329-147">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1f329-147">passcodeExpirationDays</span></span>|<span data-ttu-id="1f329-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1f329-148">Int32</span></span>|<span data-ttu-id="1f329-149">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="1f329-149">Number of days before the passcode expires.</span></span> <span data-ttu-id="1f329-150">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="1f329-150">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="1f329-151">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1f329-151">passcodeMinimumLength</span></span>|<span data-ttu-id="1f329-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1f329-152">Int32</span></span>|<span data-ttu-id="1f329-153">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="1f329-153">Minimum length of passcode.</span></span> <span data-ttu-id="1f329-154">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="1f329-154">Valid values 4 to 14</span></span>|
|<span data-ttu-id="1f329-155">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1f329-155">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1f329-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1f329-156">Int32</span></span>|<span data-ttu-id="1f329-157">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="1f329-157">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="1f329-158">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="1f329-158">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="1f329-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1f329-159">Int32</span></span>|<span data-ttu-id="1f329-160">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="1f329-160">Number of previous passcodes to block.</span></span> <span data-ttu-id="1f329-161">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="1f329-161">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1f329-162">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1f329-162">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="1f329-163">Int32</span><span class="sxs-lookup"><span data-stu-id="1f329-163">Int32</span></span>|<span data-ttu-id="1f329-164">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="1f329-164">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="1f329-165">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="1f329-165">passcodeRequiredType</span></span>|[<span data-ttu-id="1f329-166">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1f329-166">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1f329-167">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="1f329-167">The required passcode type.</span></span> <span data-ttu-id="1f329-168">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1f329-168">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1f329-169">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="1f329-169">passcodeRequired</span></span>|<span data-ttu-id="1f329-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f329-170">Boolean</span></span>|<span data-ttu-id="1f329-171">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="1f329-171">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="1f329-172">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1f329-172">osMinimumVersion</span></span>|<span data-ttu-id="1f329-173">String</span><span class="sxs-lookup"><span data-stu-id="1f329-173">String</span></span>|<span data-ttu-id="1f329-174">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="1f329-174">Minimum IOS version.</span></span>|
|<span data-ttu-id="1f329-175">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1f329-175">osMaximumVersion</span></span>|<span data-ttu-id="1f329-176">String</span><span class="sxs-lookup"><span data-stu-id="1f329-176">String</span></span>|<span data-ttu-id="1f329-177">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="1f329-177">Maximum IOS version.</span></span>|
|<span data-ttu-id="1f329-178">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="1f329-178">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="1f329-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f329-179">Boolean</span></span>|<span data-ttu-id="1f329-180">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="1f329-180">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="1f329-181">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1f329-181">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="1f329-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f329-182">Boolean</span></span>|<span data-ttu-id="1f329-183">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="1f329-183">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="1f329-184">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="1f329-184">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="1f329-185">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="1f329-185">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="1f329-186">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="1f329-186">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1f329-187">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1f329-187">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1f329-188">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="1f329-188">managedEmailProfileRequired</span></span>|<span data-ttu-id="1f329-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f329-189">Boolean</span></span>|<span data-ttu-id="1f329-190">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1f329-190">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="1f329-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f329-191">Response</span></span>
<span data-ttu-id="1f329-192">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1f329-192">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f329-193">Пример</span><span class="sxs-lookup"><span data-stu-id="1f329-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f329-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f329-194">Request</span></span>
<span data-ttu-id="1f329-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f329-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="1f329-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f329-196">Response</span></span>
<span data-ttu-id="1f329-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f329-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









