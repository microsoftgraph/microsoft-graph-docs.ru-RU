---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14e5b083e724faa55483018f5687af89de5232e4
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895338"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="cf952-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cf952-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="cf952-104">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf952-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf952-105">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf952-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf952-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cf952-106">Prerequisites</span></span>
<span data-ttu-id="cf952-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf952-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf952-109">Permission type</span></span>|<span data-ttu-id="cf952-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf952-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf952-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf952-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf952-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf952-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf952-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf952-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf952-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf952-114">Not supported.</span></span>|
|<span data-ttu-id="cf952-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf952-115">Application</span></span>|<span data-ttu-id="cf952-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf952-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf952-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf952-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cf952-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf952-118">Request headers</span></span>
|<span data-ttu-id="cf952-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf952-119">Header</span></span>|<span data-ttu-id="cf952-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cf952-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf952-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf952-121">Authorization</span></span>|<span data-ttu-id="cf952-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf952-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf952-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf952-123">Accept</span></span>|<span data-ttu-id="cf952-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf952-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf952-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf952-125">Request body</span></span>
<span data-ttu-id="cf952-126">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf952-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="cf952-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="cf952-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="cf952-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf952-128">Property</span></span>|<span data-ttu-id="cf952-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cf952-129">Type</span></span>|<span data-ttu-id="cf952-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cf952-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf952-131">description</span><span class="sxs-lookup"><span data-stu-id="cf952-131">description</span></span>|<span data-ttu-id="cf952-132">String</span><span class="sxs-lookup"><span data-stu-id="cf952-132">String</span></span>|<span data-ttu-id="cf952-133">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf952-133">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf952-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf952-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf952-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cf952-135">displayName</span></span>|<span data-ttu-id="cf952-136">Строка</span><span class="sxs-lookup"><span data-stu-id="cf952-136">String</span></span>|<span data-ttu-id="cf952-137">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf952-137">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf952-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf952-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf952-139">version</span><span class="sxs-lookup"><span data-stu-id="cf952-139">version</span></span>|<span data-ttu-id="cf952-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cf952-140">Int32</span></span>|<span data-ttu-id="cf952-141">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf952-141">Version of the device configuration.</span></span> <span data-ttu-id="cf952-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf952-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf952-143">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cf952-143">passcodeBlockSimple</span></span>|<span data-ttu-id="cf952-144">Логический</span><span class="sxs-lookup"><span data-stu-id="cf952-144">Boolean</span></span>|<span data-ttu-id="cf952-145">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="cf952-145">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="cf952-146">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cf952-146">passcodeExpirationDays</span></span>|<span data-ttu-id="cf952-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cf952-147">Int32</span></span>|<span data-ttu-id="cf952-148">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cf952-148">Number of days before the passcode expires.</span></span> <span data-ttu-id="cf952-149">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="cf952-149">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="cf952-150">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cf952-150">passcodeMinimumLength</span></span>|<span data-ttu-id="cf952-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cf952-151">Int32</span></span>|<span data-ttu-id="cf952-152">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cf952-152">Minimum length of passcode.</span></span> <span data-ttu-id="cf952-153">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="cf952-153">Valid values 4 to 14</span></span>|
|<span data-ttu-id="cf952-154">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cf952-154">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cf952-155">Int32</span><span class="sxs-lookup"><span data-stu-id="cf952-155">Int32</span></span>|<span data-ttu-id="cf952-156">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="cf952-156">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="cf952-157">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="cf952-157">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="cf952-158">Int32</span><span class="sxs-lookup"><span data-stu-id="cf952-158">Int32</span></span>|<span data-ttu-id="cf952-159">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="cf952-159">Number of previous passcodes to block.</span></span> <span data-ttu-id="cf952-160">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="cf952-160">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cf952-161">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cf952-161">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="cf952-162">Int32</span><span class="sxs-lookup"><span data-stu-id="cf952-162">Int32</span></span>|<span data-ttu-id="cf952-163">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="cf952-163">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cf952-164">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="cf952-164">passcodeRequiredType</span></span>|[<span data-ttu-id="cf952-165">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="cf952-165">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cf952-166">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cf952-166">The required passcode type.</span></span> <span data-ttu-id="cf952-167">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="cf952-167">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cf952-168">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="cf952-168">passcodeRequired</span></span>|<span data-ttu-id="cf952-169">Логический</span><span class="sxs-lookup"><span data-stu-id="cf952-169">Boolean</span></span>|<span data-ttu-id="cf952-170">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="cf952-170">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="cf952-171">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cf952-171">osMinimumVersion</span></span>|<span data-ttu-id="cf952-172">String</span><span class="sxs-lookup"><span data-stu-id="cf952-172">String</span></span>|<span data-ttu-id="cf952-173">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="cf952-173">Minimum IOS version.</span></span>|
|<span data-ttu-id="cf952-174">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cf952-174">osMaximumVersion</span></span>|<span data-ttu-id="cf952-175">String</span><span class="sxs-lookup"><span data-stu-id="cf952-175">String</span></span>|<span data-ttu-id="cf952-176">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="cf952-176">Maximum IOS version.</span></span>|
|<span data-ttu-id="cf952-177">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="cf952-177">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="cf952-178">Логический</span><span class="sxs-lookup"><span data-stu-id="cf952-178">Boolean</span></span>|<span data-ttu-id="cf952-179">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="cf952-179">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="cf952-180">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cf952-180">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cf952-181">Логический</span><span class="sxs-lookup"><span data-stu-id="cf952-181">Boolean</span></span>|<span data-ttu-id="cf952-182">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="cf952-182">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="cf952-183">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cf952-183">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cf952-184">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="cf952-184">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cf952-185">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="cf952-185">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cf952-186">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="cf952-186">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cf952-187">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="cf952-187">managedEmailProfileRequired</span></span>|<span data-ttu-id="cf952-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf952-188">Boolean</span></span>|<span data-ttu-id="cf952-189">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cf952-189">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="cf952-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf952-190">Response</span></span>
<span data-ttu-id="cf952-191">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf952-191">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf952-192">Пример</span><span class="sxs-lookup"><span data-stu-id="cf952-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf952-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf952-193">Request</span></span>
<span data-ttu-id="cf952-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf952-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf952-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf952-195">Response</span></span>
<span data-ttu-id="cf952-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf952-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




