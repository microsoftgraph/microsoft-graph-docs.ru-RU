---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: fd039005455c94cf55fa1afe21eee33fde9b4588
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346174"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="265ae-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="265ae-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="265ae-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="265ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="265ae-105">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="265ae-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="265ae-106">Prerequisites</span></span>
<span data-ttu-id="265ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="265ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="265ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="265ae-109">Permission type</span></span>|<span data-ttu-id="265ae-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="265ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="265ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="265ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="265ae-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="265ae-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="265ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="265ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="265ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="265ae-114">Not supported.</span></span>|
|<span data-ttu-id="265ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="265ae-115">Application</span></span>|<span data-ttu-id="265ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="265ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="265ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="265ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="265ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="265ae-118">Request headers</span></span>
|<span data-ttu-id="265ae-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="265ae-119">Header</span></span>|<span data-ttu-id="265ae-120">Значение</span><span class="sxs-lookup"><span data-stu-id="265ae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="265ae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="265ae-121">Authorization</span></span>|<span data-ttu-id="265ae-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="265ae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="265ae-123">Accept</span><span class="sxs-lookup"><span data-stu-id="265ae-123">Accept</span></span>|<span data-ttu-id="265ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="265ae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="265ae-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="265ae-125">Request body</span></span>
<span data-ttu-id="265ae-126">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="265ae-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="265ae-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="265ae-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="265ae-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="265ae-128">Property</span></span>|<span data-ttu-id="265ae-129">Тип</span><span class="sxs-lookup"><span data-stu-id="265ae-129">Type</span></span>|<span data-ttu-id="265ae-130">Описание</span><span class="sxs-lookup"><span data-stu-id="265ae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="265ae-131">id</span><span class="sxs-lookup"><span data-stu-id="265ae-131">id</span></span>|<span data-ttu-id="265ae-132">Строка</span><span class="sxs-lookup"><span data-stu-id="265ae-132">String</span></span>|<span data-ttu-id="265ae-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="265ae-133">Key of the entity.</span></span> <span data-ttu-id="265ae-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="265ae-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="265ae-135">createdDateTime</span></span>|<span data-ttu-id="265ae-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="265ae-136">DateTimeOffset</span></span>|<span data-ttu-id="265ae-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="265ae-137">DateTime the object was created.</span></span> <span data-ttu-id="265ae-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="265ae-139">описание</span><span class="sxs-lookup"><span data-stu-id="265ae-139">description</span></span>|<span data-ttu-id="265ae-140">Строка</span><span class="sxs-lookup"><span data-stu-id="265ae-140">String</span></span>|<span data-ttu-id="265ae-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="265ae-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="265ae-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="265ae-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="265ae-143">lastModifiedDateTime</span></span>|<span data-ttu-id="265ae-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="265ae-144">DateTimeOffset</span></span>|<span data-ttu-id="265ae-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="265ae-145">DateTime the object was last modified.</span></span> <span data-ttu-id="265ae-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="265ae-147">displayName</span><span class="sxs-lookup"><span data-stu-id="265ae-147">displayName</span></span>|<span data-ttu-id="265ae-148">Строка</span><span class="sxs-lookup"><span data-stu-id="265ae-148">String</span></span>|<span data-ttu-id="265ae-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="265ae-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="265ae-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="265ae-151">version</span><span class="sxs-lookup"><span data-stu-id="265ae-151">version</span></span>|<span data-ttu-id="265ae-152">Int32</span><span class="sxs-lookup"><span data-stu-id="265ae-152">Int32</span></span>|<span data-ttu-id="265ae-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="265ae-153">Version of the device configuration.</span></span> <span data-ttu-id="265ae-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="265ae-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="265ae-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="265ae-155">passcodeBlockSimple</span></span>|<span data-ttu-id="265ae-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="265ae-156">Boolean</span></span>|<span data-ttu-id="265ae-157">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="265ae-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="265ae-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="265ae-158">passcodeExpirationDays</span></span>|<span data-ttu-id="265ae-159">Int32</span><span class="sxs-lookup"><span data-stu-id="265ae-159">Int32</span></span>|<span data-ttu-id="265ae-160">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="265ae-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="265ae-161">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="265ae-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="265ae-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="265ae-162">passcodeMinimumLength</span></span>|<span data-ttu-id="265ae-163">Int32</span><span class="sxs-lookup"><span data-stu-id="265ae-163">Int32</span></span>|<span data-ttu-id="265ae-164">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="265ae-164">Minimum length of passcode.</span></span> <span data-ttu-id="265ae-165">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="265ae-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="265ae-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="265ae-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="265ae-167">Int32</span><span class="sxs-lookup"><span data-stu-id="265ae-167">Int32</span></span>|<span data-ttu-id="265ae-168">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="265ae-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="265ae-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="265ae-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="265ae-170">Int32</span><span class="sxs-lookup"><span data-stu-id="265ae-170">Int32</span></span>|<span data-ttu-id="265ae-171">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="265ae-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="265ae-172">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="265ae-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="265ae-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="265ae-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="265ae-174">Int32</span><span class="sxs-lookup"><span data-stu-id="265ae-174">Int32</span></span>|<span data-ttu-id="265ae-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="265ae-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="265ae-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="265ae-176">passcodeRequiredType</span></span>|[<span data-ttu-id="265ae-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="265ae-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="265ae-178">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="265ae-178">The required passcode type.</span></span> <span data-ttu-id="265ae-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="265ae-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="265ae-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="265ae-180">passcodeRequired</span></span>|<span data-ttu-id="265ae-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="265ae-181">Boolean</span></span>|<span data-ttu-id="265ae-182">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="265ae-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="265ae-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="265ae-183">osMinimumVersion</span></span>|<span data-ttu-id="265ae-184">String</span><span class="sxs-lookup"><span data-stu-id="265ae-184">String</span></span>|<span data-ttu-id="265ae-185">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="265ae-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="265ae-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="265ae-186">osMaximumVersion</span></span>|<span data-ttu-id="265ae-187">String</span><span class="sxs-lookup"><span data-stu-id="265ae-187">String</span></span>|<span data-ttu-id="265ae-188">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="265ae-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="265ae-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="265ae-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="265ae-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="265ae-190">Boolean</span></span>|<span data-ttu-id="265ae-191">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="265ae-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="265ae-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="265ae-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="265ae-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="265ae-193">Boolean</span></span>|<span data-ttu-id="265ae-194">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="265ae-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="265ae-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="265ae-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="265ae-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="265ae-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="265ae-197">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="265ae-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="265ae-198">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="265ae-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="265ae-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="265ae-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="265ae-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="265ae-200">Boolean</span></span>|<span data-ttu-id="265ae-201">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="265ae-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="265ae-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="265ae-202">Response</span></span>
<span data-ttu-id="265ae-203">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="265ae-203">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="265ae-204">Пример</span><span class="sxs-lookup"><span data-stu-id="265ae-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="265ae-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="265ae-205">Request</span></span>
<span data-ttu-id="265ae-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="265ae-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="265ae-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="265ae-207">Response</span></span>
<span data-ttu-id="265ae-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="265ae-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



