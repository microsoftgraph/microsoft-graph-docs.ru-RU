---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 3b6589601622015f589c10f2ed839117b4755269
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305126"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="3b6f6-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3b6f6-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="3b6f6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b6f6-105">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b6f6-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3b6f6-106">Prerequisites</span></span>
<span data-ttu-id="3b6f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b6f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b6f6-109">Permission type</span></span>|<span data-ttu-id="3b6f6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b6f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b6f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b6f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b6f6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b6f6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b6f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b6f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b6f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-114">Not supported.</span></span>|
|<span data-ttu-id="3b6f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b6f6-115">Application</span></span>|<span data-ttu-id="3b6f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b6f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b6f6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3b6f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b6f6-118">Request headers</span></span>
|<span data-ttu-id="3b6f6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b6f6-119">Header</span></span>|<span data-ttu-id="3b6f6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3b6f6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b6f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b6f6-121">Authorization</span></span>|<span data-ttu-id="3b6f6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b6f6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b6f6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3b6f6-123">Accept</span></span>|<span data-ttu-id="3b6f6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b6f6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b6f6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b6f6-125">Request body</span></span>
<span data-ttu-id="3b6f6-126">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="3b6f6-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="3b6f6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b6f6-128">Property</span></span>|<span data-ttu-id="3b6f6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3b6f6-129">Type</span></span>|<span data-ttu-id="3b6f6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b6f6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b6f6-131">id</span><span class="sxs-lookup"><span data-stu-id="3b6f6-131">id</span></span>|<span data-ttu-id="3b6f6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3b6f6-132">String</span></span>|<span data-ttu-id="3b6f6-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-133">Key of the entity.</span></span> <span data-ttu-id="3b6f6-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b6f6-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b6f6-135">createdDateTime</span></span>|<span data-ttu-id="3b6f6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b6f6-136">DateTimeOffset</span></span>|<span data-ttu-id="3b6f6-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-137">DateTime the object was created.</span></span> <span data-ttu-id="3b6f6-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b6f6-139">описание</span><span class="sxs-lookup"><span data-stu-id="3b6f6-139">description</span></span>|<span data-ttu-id="3b6f6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3b6f6-140">String</span></span>|<span data-ttu-id="3b6f6-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b6f6-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b6f6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b6f6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3b6f6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b6f6-144">DateTimeOffset</span></span>|<span data-ttu-id="3b6f6-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-145">DateTime the object was last modified.</span></span> <span data-ttu-id="3b6f6-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b6f6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3b6f6-147">displayName</span></span>|<span data-ttu-id="3b6f6-148">Строка</span><span class="sxs-lookup"><span data-stu-id="3b6f6-148">String</span></span>|<span data-ttu-id="3b6f6-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b6f6-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b6f6-151">version</span><span class="sxs-lookup"><span data-stu-id="3b6f6-151">version</span></span>|<span data-ttu-id="3b6f6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3b6f6-152">Int32</span></span>|<span data-ttu-id="3b6f6-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-153">Version of the device configuration.</span></span> <span data-ttu-id="3b6f6-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b6f6-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b6f6-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3b6f6-155">passcodeBlockSimple</span></span>|<span data-ttu-id="3b6f6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b6f6-156">Boolean</span></span>|<span data-ttu-id="3b6f6-157">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="3b6f6-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3b6f6-158">passcodeExpirationDays</span></span>|<span data-ttu-id="3b6f6-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3b6f6-159">Int32</span></span>|<span data-ttu-id="3b6f6-160">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="3b6f6-161">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="3b6f6-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3b6f6-162">passcodeMinimumLength</span></span>|<span data-ttu-id="3b6f6-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3b6f6-163">Int32</span></span>|<span data-ttu-id="3b6f6-164">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-164">Minimum length of passcode.</span></span> <span data-ttu-id="3b6f6-165">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="3b6f6-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3b6f6-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3b6f6-167">Int32</span><span class="sxs-lookup"><span data-stu-id="3b6f6-167">Int32</span></span>|<span data-ttu-id="3b6f6-168">Период бездействия (в минутах), по истечении которого будет запрашиваться секретный код.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="3b6f6-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="3b6f6-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="3b6f6-170">Int32</span><span class="sxs-lookup"><span data-stu-id="3b6f6-170">Int32</span></span>|<span data-ttu-id="3b6f6-171">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="3b6f6-172">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3b6f6-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3b6f6-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="3b6f6-174">Int32</span><span class="sxs-lookup"><span data-stu-id="3b6f6-174">Int32</span></span>|<span data-ttu-id="3b6f6-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3b6f6-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="3b6f6-176">passcodeRequiredType</span></span>|[<span data-ttu-id="3b6f6-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3b6f6-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3b6f6-178">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-178">The required passcode type.</span></span> <span data-ttu-id="3b6f6-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3b6f6-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="3b6f6-180">passcodeRequired</span></span>|<span data-ttu-id="3b6f6-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b6f6-181">Boolean</span></span>|<span data-ttu-id="3b6f6-182">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="3b6f6-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3b6f6-183">osMinimumVersion</span></span>|<span data-ttu-id="3b6f6-184">String</span><span class="sxs-lookup"><span data-stu-id="3b6f6-184">String</span></span>|<span data-ttu-id="3b6f6-185">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="3b6f6-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3b6f6-186">osMaximumVersion</span></span>|<span data-ttu-id="3b6f6-187">String</span><span class="sxs-lookup"><span data-stu-id="3b6f6-187">String</span></span>|<span data-ttu-id="3b6f6-188">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="3b6f6-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="3b6f6-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="3b6f6-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b6f6-190">Boolean</span></span>|<span data-ttu-id="3b6f6-191">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="3b6f6-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3b6f6-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3b6f6-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b6f6-193">Boolean</span></span>|<span data-ttu-id="3b6f6-194">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="3b6f6-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3b6f6-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3b6f6-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3b6f6-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3b6f6-197">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3b6f6-198">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3b6f6-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="3b6f6-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="3b6f6-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b6f6-200">Boolean</span></span>|<span data-ttu-id="3b6f6-201">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="3b6f6-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b6f6-202">Response</span></span>
<span data-ttu-id="3b6f6-203">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b6f6-204">Пример</span><span class="sxs-lookup"><span data-stu-id="3b6f6-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b6f6-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b6f6-205">Request</span></span>
<span data-ttu-id="3b6f6-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b6f6-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b6f6-207">Response</span></span>
<span data-ttu-id="3b6f6-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3b6f6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



