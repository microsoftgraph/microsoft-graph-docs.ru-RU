---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51f0658ab4e1da860048b70ca1c168d8798c173b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514643"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="82946-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="82946-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="82946-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82946-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82946-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82946-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82946-106">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82946-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82946-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="82946-107">Prerequisites</span></span>
<span data-ttu-id="82946-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82946-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82946-110">Permission type</span></span>|<span data-ttu-id="82946-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82946-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82946-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82946-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82946-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82946-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82946-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82946-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82946-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82946-115">Not supported.</span></span>|
|<span data-ttu-id="82946-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82946-116">Application</span></span>|<span data-ttu-id="82946-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82946-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82946-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82946-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="82946-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82946-119">Request headers</span></span>
|<span data-ttu-id="82946-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82946-120">Header</span></span>|<span data-ttu-id="82946-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82946-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82946-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82946-122">Authorization</span></span>|<span data-ttu-id="82946-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82946-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82946-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82946-124">Accept</span></span>|<span data-ttu-id="82946-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82946-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82946-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82946-126">Request body</span></span>
<span data-ttu-id="82946-127">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82946-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="82946-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="82946-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="82946-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82946-129">Property</span></span>|<span data-ttu-id="82946-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82946-130">Type</span></span>|<span data-ttu-id="82946-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82946-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82946-132">description</span><span class="sxs-lookup"><span data-stu-id="82946-132">description</span></span>|<span data-ttu-id="82946-133">String</span><span class="sxs-lookup"><span data-stu-id="82946-133">String</span></span>|<span data-ttu-id="82946-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82946-134">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82946-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82946-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82946-136">displayName</span><span class="sxs-lookup"><span data-stu-id="82946-136">displayName</span></span>|<span data-ttu-id="82946-137">Строка</span><span class="sxs-lookup"><span data-stu-id="82946-137">String</span></span>|<span data-ttu-id="82946-138">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82946-138">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82946-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82946-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82946-140">version</span><span class="sxs-lookup"><span data-stu-id="82946-140">version</span></span>|<span data-ttu-id="82946-141">Int32</span><span class="sxs-lookup"><span data-stu-id="82946-141">Int32</span></span>|<span data-ttu-id="82946-142">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82946-142">Version of the device configuration.</span></span> <span data-ttu-id="82946-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82946-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82946-144">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="82946-144">passcodeBlockSimple</span></span>|<span data-ttu-id="82946-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="82946-145">Boolean</span></span>|<span data-ttu-id="82946-146">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="82946-146">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="82946-147">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="82946-147">passcodeExpirationDays</span></span>|<span data-ttu-id="82946-148">Int32</span><span class="sxs-lookup"><span data-stu-id="82946-148">Int32</span></span>|<span data-ttu-id="82946-149">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="82946-149">Number of days before the passcode expires.</span></span> <span data-ttu-id="82946-150">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="82946-150">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="82946-151">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82946-151">passcodeMinimumLength</span></span>|<span data-ttu-id="82946-152">Int32</span><span class="sxs-lookup"><span data-stu-id="82946-152">Int32</span></span>|<span data-ttu-id="82946-153">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="82946-153">Minimum length of passcode.</span></span> <span data-ttu-id="82946-154">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="82946-154">Valid values 4 to 14</span></span>|
|<span data-ttu-id="82946-155">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="82946-155">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="82946-156">Int32</span><span class="sxs-lookup"><span data-stu-id="82946-156">Int32</span></span>|<span data-ttu-id="82946-157">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="82946-157">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="82946-158">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="82946-158">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="82946-159">Int32</span><span class="sxs-lookup"><span data-stu-id="82946-159">Int32</span></span>|<span data-ttu-id="82946-160">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="82946-160">Number of previous passcodes to block.</span></span> <span data-ttu-id="82946-161">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="82946-161">Valid values 1 to 24</span></span>|
|<span data-ttu-id="82946-162">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="82946-162">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="82946-163">Int32</span><span class="sxs-lookup"><span data-stu-id="82946-163">Int32</span></span>|<span data-ttu-id="82946-164">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="82946-164">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="82946-165">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="82946-165">passcodeRequiredType</span></span>|[<span data-ttu-id="82946-166">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="82946-166">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="82946-167">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="82946-167">The required passcode type.</span></span> <span data-ttu-id="82946-168">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="82946-168">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="82946-169">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="82946-169">passcodeRequired</span></span>|<span data-ttu-id="82946-170">Логический</span><span class="sxs-lookup"><span data-stu-id="82946-170">Boolean</span></span>|<span data-ttu-id="82946-171">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="82946-171">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="82946-172">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="82946-172">osMinimumVersion</span></span>|<span data-ttu-id="82946-173">Строка</span><span class="sxs-lookup"><span data-stu-id="82946-173">String</span></span>|<span data-ttu-id="82946-174">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="82946-174">Minimum IOS version.</span></span>|
|<span data-ttu-id="82946-175">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="82946-175">osMaximumVersion</span></span>|<span data-ttu-id="82946-176">String</span><span class="sxs-lookup"><span data-stu-id="82946-176">String</span></span>|<span data-ttu-id="82946-177">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="82946-177">Maximum IOS version.</span></span>|
|<span data-ttu-id="82946-178">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="82946-178">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="82946-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="82946-179">Boolean</span></span>|<span data-ttu-id="82946-180">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="82946-180">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="82946-181">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="82946-181">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="82946-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="82946-182">Boolean</span></span>|<span data-ttu-id="82946-183">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="82946-183">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="82946-184">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="82946-184">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="82946-185">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="82946-185">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="82946-186">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="82946-186">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="82946-187">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="82946-187">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="82946-188">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="82946-188">managedEmailProfileRequired</span></span>|<span data-ttu-id="82946-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="82946-189">Boolean</span></span>|<span data-ttu-id="82946-190">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82946-190">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="82946-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="82946-191">Response</span></span>
<span data-ttu-id="82946-192">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="82946-192">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82946-193">Пример</span><span class="sxs-lookup"><span data-stu-id="82946-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="82946-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="82946-194">Request</span></span>
<span data-ttu-id="82946-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82946-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82946-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="82946-196">Response</span></span>
<span data-ttu-id="82946-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82946-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




