---
title: Create macOSCompliancePolicy
description: Создание объекта macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b489aaabca59513e6f14baf52bbfb0e046ac223d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811426"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="14584-103">Create macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="14584-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="14584-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14584-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14584-105">Создание объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14584-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="14584-106">Prerequisites</span></span>
<span data-ttu-id="14584-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14584-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14584-109">Permission type</span></span>|<span data-ttu-id="14584-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14584-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14584-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14584-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14584-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14584-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14584-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14584-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14584-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14584-114">Not supported.</span></span>|
|<span data-ttu-id="14584-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14584-115">Application</span></span>|<span data-ttu-id="14584-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14584-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14584-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14584-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="14584-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14584-118">Request headers</span></span>
|<span data-ttu-id="14584-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14584-119">Header</span></span>|<span data-ttu-id="14584-120">Значение</span><span class="sxs-lookup"><span data-stu-id="14584-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14584-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="14584-121">Authorization</span></span>|<span data-ttu-id="14584-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="14584-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14584-123">Accept</span><span class="sxs-lookup"><span data-stu-id="14584-123">Accept</span></span>|<span data-ttu-id="14584-124">application/json</span><span class="sxs-lookup"><span data-stu-id="14584-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14584-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14584-125">Request body</span></span>
<span data-ttu-id="14584-126">В теле запроса добавьте представление объекта macOSCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14584-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="14584-127">Ниже показаны свойства, которые необходимо указывать при создании объекта macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="14584-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="14584-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="14584-128">Property</span></span>|<span data-ttu-id="14584-129">Тип</span><span class="sxs-lookup"><span data-stu-id="14584-129">Type</span></span>|<span data-ttu-id="14584-130">Описание</span><span class="sxs-lookup"><span data-stu-id="14584-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14584-131">id</span><span class="sxs-lookup"><span data-stu-id="14584-131">id</span></span>|<span data-ttu-id="14584-132">Строка</span><span class="sxs-lookup"><span data-stu-id="14584-132">String</span></span>|<span data-ttu-id="14584-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14584-133">Key of the entity.</span></span> <span data-ttu-id="14584-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="14584-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14584-135">createdDateTime</span></span>|<span data-ttu-id="14584-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14584-136">DateTimeOffset</span></span>|<span data-ttu-id="14584-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="14584-137">DateTime the object was created.</span></span> <span data-ttu-id="14584-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="14584-139">описание</span><span class="sxs-lookup"><span data-stu-id="14584-139">description</span></span>|<span data-ttu-id="14584-140">Строка</span><span class="sxs-lookup"><span data-stu-id="14584-140">String</span></span>|<span data-ttu-id="14584-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14584-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14584-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="14584-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14584-143">lastModifiedDateTime</span></span>|<span data-ttu-id="14584-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14584-144">DateTimeOffset</span></span>|<span data-ttu-id="14584-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="14584-145">DateTime the object was last modified.</span></span> <span data-ttu-id="14584-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="14584-147">displayName</span><span class="sxs-lookup"><span data-stu-id="14584-147">displayName</span></span>|<span data-ttu-id="14584-148">Строка</span><span class="sxs-lookup"><span data-stu-id="14584-148">String</span></span>|<span data-ttu-id="14584-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14584-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14584-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="14584-151">version</span><span class="sxs-lookup"><span data-stu-id="14584-151">version</span></span>|<span data-ttu-id="14584-152">Int32</span><span class="sxs-lookup"><span data-stu-id="14584-152">Int32</span></span>|<span data-ttu-id="14584-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14584-153">Version of the device configuration.</span></span> <span data-ttu-id="14584-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="14584-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="14584-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="14584-155">passwordRequired</span></span>|<span data-ttu-id="14584-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="14584-156">Boolean</span></span>|<span data-ttu-id="14584-157">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="14584-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="14584-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="14584-158">passwordBlockSimple</span></span>|<span data-ttu-id="14584-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="14584-159">Boolean</span></span>|<span data-ttu-id="14584-160">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="14584-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="14584-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="14584-161">passwordExpirationDays</span></span>|<span data-ttu-id="14584-162">Int32</span><span class="sxs-lookup"><span data-stu-id="14584-162">Int32</span></span>|<span data-ttu-id="14584-163">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="14584-163">Number of days before the password expires.</span></span> <span data-ttu-id="14584-164">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="14584-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="14584-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="14584-165">passwordMinimumLength</span></span>|<span data-ttu-id="14584-166">Int32</span><span class="sxs-lookup"><span data-stu-id="14584-166">Int32</span></span>|<span data-ttu-id="14584-167">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="14584-167">Minimum length of password.</span></span> <span data-ttu-id="14584-168">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="14584-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="14584-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="14584-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="14584-170">Int32</span><span class="sxs-lookup"><span data-stu-id="14584-170">Int32</span></span>|<span data-ttu-id="14584-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="14584-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="14584-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="14584-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="14584-173">Int32</span><span class="sxs-lookup"><span data-stu-id="14584-173">Int32</span></span>|<span data-ttu-id="14584-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="14584-174">Number of previous passwords to block.</span></span> <span data-ttu-id="14584-175">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="14584-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="14584-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="14584-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="14584-177">Int32</span><span class="sxs-lookup"><span data-stu-id="14584-177">Int32</span></span>|<span data-ttu-id="14584-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="14584-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="14584-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="14584-179">passwordRequiredType</span></span>|[<span data-ttu-id="14584-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="14584-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="14584-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="14584-181">The required password type.</span></span> <span data-ttu-id="14584-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="14584-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="14584-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="14584-183">osMinimumVersion</span></span>|<span data-ttu-id="14584-184">String</span><span class="sxs-lookup"><span data-stu-id="14584-184">String</span></span>|<span data-ttu-id="14584-185">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="14584-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="14584-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="14584-186">osMaximumVersion</span></span>|<span data-ttu-id="14584-187">String</span><span class="sxs-lookup"><span data-stu-id="14584-187">String</span></span>|<span data-ttu-id="14584-188">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="14584-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="14584-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="14584-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="14584-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="14584-190">Boolean</span></span>|<span data-ttu-id="14584-191">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="14584-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="14584-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="14584-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="14584-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="14584-193">Boolean</span></span>|<span data-ttu-id="14584-194">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="14584-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="14584-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="14584-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="14584-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="14584-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="14584-197">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="14584-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="14584-198">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="14584-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="14584-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="14584-199">storageRequireEncryption</span></span>|<span data-ttu-id="14584-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="14584-200">Boolean</span></span>|<span data-ttu-id="14584-201">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="14584-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="14584-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="14584-202">firewallEnabled</span></span>|<span data-ttu-id="14584-203">Логический</span><span class="sxs-lookup"><span data-stu-id="14584-203">Boolean</span></span>|<span data-ttu-id="14584-204">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="14584-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="14584-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="14584-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="14584-206">Логический</span><span class="sxs-lookup"><span data-stu-id="14584-206">Boolean</span></span>|<span data-ttu-id="14584-207">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="14584-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="14584-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="14584-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="14584-209">Логический</span><span class="sxs-lookup"><span data-stu-id="14584-209">Boolean</span></span>|<span data-ttu-id="14584-210">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="14584-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="14584-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="14584-211">Response</span></span>
<span data-ttu-id="14584-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14584-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14584-213">Пример</span><span class="sxs-lookup"><span data-stu-id="14584-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="14584-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="14584-214">Request</span></span>
<span data-ttu-id="14584-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14584-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="14584-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="14584-216">Response</span></span>
<span data-ttu-id="14584-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="14584-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



