---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fccf80d259562c6064a8307c601d477dfc8c3693
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759263"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="5408f-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5408f-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="5408f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5408f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5408f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5408f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5408f-106">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5408f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5408f-107">Prerequisites</span></span>
<span data-ttu-id="5408f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5408f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5408f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5408f-110">Permission type</span></span>|<span data-ttu-id="5408f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5408f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5408f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5408f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5408f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5408f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5408f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5408f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5408f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5408f-115">Not supported.</span></span>|
|<span data-ttu-id="5408f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5408f-116">Application</span></span>|<span data-ttu-id="5408f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5408f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5408f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5408f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5408f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5408f-119">Request headers</span></span>
|<span data-ttu-id="5408f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5408f-120">Header</span></span>|<span data-ttu-id="5408f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5408f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5408f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5408f-122">Authorization</span></span>|<span data-ttu-id="5408f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5408f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5408f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5408f-124">Accept</span></span>|<span data-ttu-id="5408f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5408f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5408f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5408f-126">Request body</span></span>
<span data-ttu-id="5408f-127">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5408f-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="5408f-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5408f-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="5408f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5408f-129">Property</span></span>|<span data-ttu-id="5408f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5408f-130">Type</span></span>|<span data-ttu-id="5408f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5408f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5408f-132">id</span><span class="sxs-lookup"><span data-stu-id="5408f-132">id</span></span>|<span data-ttu-id="5408f-133">String</span><span class="sxs-lookup"><span data-stu-id="5408f-133">String</span></span>|<span data-ttu-id="5408f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5408f-134">Key of the entity.</span></span> <span data-ttu-id="5408f-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5408f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5408f-136">createdDateTime</span></span>|<span data-ttu-id="5408f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5408f-137">DateTimeOffset</span></span>|<span data-ttu-id="5408f-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5408f-138">DateTime the object was created.</span></span> <span data-ttu-id="5408f-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5408f-140">description</span><span class="sxs-lookup"><span data-stu-id="5408f-140">description</span></span>|<span data-ttu-id="5408f-141">String</span><span class="sxs-lookup"><span data-stu-id="5408f-141">String</span></span>|<span data-ttu-id="5408f-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5408f-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5408f-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5408f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5408f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5408f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5408f-145">DateTimeOffset</span></span>|<span data-ttu-id="5408f-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5408f-146">DateTime the object was last modified.</span></span> <span data-ttu-id="5408f-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5408f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5408f-148">displayName</span></span>|<span data-ttu-id="5408f-149">String</span><span class="sxs-lookup"><span data-stu-id="5408f-149">String</span></span>|<span data-ttu-id="5408f-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5408f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5408f-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5408f-152">version</span><span class="sxs-lookup"><span data-stu-id="5408f-152">version</span></span>|<span data-ttu-id="5408f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5408f-153">Int32</span></span>|<span data-ttu-id="5408f-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5408f-154">Version of the device configuration.</span></span> <span data-ttu-id="5408f-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5408f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5408f-156">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5408f-156">passcodeBlockSimple</span></span>|<span data-ttu-id="5408f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="5408f-157">Boolean</span></span>|<span data-ttu-id="5408f-158">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="5408f-158">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="5408f-159">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5408f-159">passcodeExpirationDays</span></span>|<span data-ttu-id="5408f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5408f-160">Int32</span></span>|<span data-ttu-id="5408f-161">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="5408f-161">Number of days before the passcode expires.</span></span> <span data-ttu-id="5408f-162">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="5408f-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="5408f-163">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5408f-163">passcodeMinimumLength</span></span>|<span data-ttu-id="5408f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5408f-164">Int32</span></span>|<span data-ttu-id="5408f-165">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="5408f-165">Minimum length of passcode.</span></span> <span data-ttu-id="5408f-166">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="5408f-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="5408f-167">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5408f-167">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5408f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5408f-168">Int32</span></span>|<span data-ttu-id="5408f-169">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="5408f-169">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="5408f-170">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="5408f-170">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="5408f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5408f-171">Int32</span></span>|<span data-ttu-id="5408f-172">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="5408f-172">Number of previous passcodes to block.</span></span> <span data-ttu-id="5408f-173">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="5408f-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5408f-174">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5408f-174">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="5408f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="5408f-175">Int32</span></span>|<span data-ttu-id="5408f-176">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5408f-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5408f-177">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="5408f-177">passcodeRequiredType</span></span>|[<span data-ttu-id="5408f-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5408f-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5408f-179">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="5408f-179">The required passcode type.</span></span> <span data-ttu-id="5408f-180">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5408f-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5408f-181">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="5408f-181">passcodeRequired</span></span>|<span data-ttu-id="5408f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5408f-182">Boolean</span></span>|<span data-ttu-id="5408f-183">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="5408f-183">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="5408f-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5408f-184">osMinimumVersion</span></span>|<span data-ttu-id="5408f-185">String</span><span class="sxs-lookup"><span data-stu-id="5408f-185">String</span></span>|<span data-ttu-id="5408f-186">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="5408f-186">Minimum IOS version.</span></span>|
|<span data-ttu-id="5408f-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5408f-187">osMaximumVersion</span></span>|<span data-ttu-id="5408f-188">String</span><span class="sxs-lookup"><span data-stu-id="5408f-188">String</span></span>|<span data-ttu-id="5408f-189">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="5408f-189">Maximum IOS version.</span></span>|
|<span data-ttu-id="5408f-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="5408f-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="5408f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="5408f-191">Boolean</span></span>|<span data-ttu-id="5408f-192">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="5408f-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="5408f-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5408f-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5408f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5408f-194">Boolean</span></span>|<span data-ttu-id="5408f-195">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="5408f-195">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="5408f-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5408f-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5408f-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="5408f-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5408f-198">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="5408f-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5408f-199">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5408f-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5408f-200">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="5408f-200">managedEmailProfileRequired</span></span>|<span data-ttu-id="5408f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5408f-201">Boolean</span></span>|<span data-ttu-id="5408f-202">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5408f-202">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="5408f-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="5408f-203">Response</span></span>
<span data-ttu-id="5408f-204">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5408f-204">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5408f-205">Пример</span><span class="sxs-lookup"><span data-stu-id="5408f-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="5408f-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="5408f-206">Request</span></span>
<span data-ttu-id="5408f-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5408f-207">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5408f-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="5408f-208">Response</span></span>
<span data-ttu-id="5408f-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5408f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




