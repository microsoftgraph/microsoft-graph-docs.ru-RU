---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 524ffd9bbaf7b6a0e5d1e912d52af8137e59049f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167699"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="4839e-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4839e-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="4839e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4839e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4839e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4839e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4839e-106">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4839e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4839e-107">Prerequisites</span></span>
<span data-ttu-id="4839e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4839e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4839e-110">Permission type</span></span>|<span data-ttu-id="4839e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4839e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4839e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4839e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4839e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4839e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4839e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4839e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4839e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4839e-115">Not supported.</span></span>|
|<span data-ttu-id="4839e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4839e-116">Application</span></span>|<span data-ttu-id="4839e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4839e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4839e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4839e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4839e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4839e-119">Request headers</span></span>
|<span data-ttu-id="4839e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4839e-120">Header</span></span>|<span data-ttu-id="4839e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4839e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4839e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4839e-122">Authorization</span></span>|<span data-ttu-id="4839e-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4839e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4839e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4839e-124">Accept</span></span>|<span data-ttu-id="4839e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4839e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4839e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4839e-126">Request body</span></span>
<span data-ttu-id="4839e-127">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4839e-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="4839e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="4839e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4839e-129">Property</span></span>|<span data-ttu-id="4839e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4839e-130">Type</span></span>|<span data-ttu-id="4839e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4839e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4839e-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4839e-132">roleScopeTagIds</span></span>|<span data-ttu-id="4839e-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4839e-133">String collection</span></span>|<span data-ttu-id="4839e-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4839e-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4839e-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-136">id</span><span class="sxs-lookup"><span data-stu-id="4839e-136">id</span></span>|<span data-ttu-id="4839e-137">String</span><span class="sxs-lookup"><span data-stu-id="4839e-137">String</span></span>|<span data-ttu-id="4839e-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4839e-138">Key of the entity.</span></span> <span data-ttu-id="4839e-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4839e-140">createdDateTime</span></span>|<span data-ttu-id="4839e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4839e-141">DateTimeOffset</span></span>|<span data-ttu-id="4839e-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4839e-142">DateTime the object was created.</span></span> <span data-ttu-id="4839e-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-144">description</span><span class="sxs-lookup"><span data-stu-id="4839e-144">description</span></span>|<span data-ttu-id="4839e-145">Строка</span><span class="sxs-lookup"><span data-stu-id="4839e-145">String</span></span>|<span data-ttu-id="4839e-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4839e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4839e-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4839e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4839e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4839e-149">DateTimeOffset</span></span>|<span data-ttu-id="4839e-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4839e-150">DateTime the object was last modified.</span></span> <span data-ttu-id="4839e-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="4839e-152">displayName</span></span>|<span data-ttu-id="4839e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="4839e-153">String</span></span>|<span data-ttu-id="4839e-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4839e-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4839e-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4839e-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-156">version</span><span class="sxs-lookup"><span data-stu-id="4839e-156">version</span></span>|<span data-ttu-id="4839e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-157">Int32</span></span>|<span data-ttu-id="4839e-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4839e-158">Version of the device configuration.</span></span> <span data-ttu-id="4839e-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4839e-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4839e-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4839e-160">passcodeBlockSimple</span></span>|<span data-ttu-id="4839e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4839e-161">Boolean</span></span>|<span data-ttu-id="4839e-162">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="4839e-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="4839e-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4839e-163">passcodeExpirationDays</span></span>|<span data-ttu-id="4839e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-164">Int32</span></span>|<span data-ttu-id="4839e-165">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="4839e-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="4839e-166">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="4839e-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4839e-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4839e-167">passcodeMinimumLength</span></span>|<span data-ttu-id="4839e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-168">Int32</span></span>|<span data-ttu-id="4839e-169">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="4839e-169">Minimum length of passcode.</span></span> <span data-ttu-id="4839e-170">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="4839e-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4839e-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4839e-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4839e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-172">Int32</span></span>|<span data-ttu-id="4839e-173">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="4839e-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="4839e-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4839e-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4839e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-175">Int32</span></span>|<span data-ttu-id="4839e-176">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="4839e-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4839e-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="4839e-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="4839e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-178">Int32</span></span>|<span data-ttu-id="4839e-179">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="4839e-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="4839e-180">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="4839e-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4839e-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4839e-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="4839e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="4839e-182">Int32</span></span>|<span data-ttu-id="4839e-183">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="4839e-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4839e-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="4839e-184">passcodeRequiredType</span></span>|[<span data-ttu-id="4839e-185">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4839e-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4839e-186">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="4839e-186">The required passcode type.</span></span> <span data-ttu-id="4839e-187">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4839e-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4839e-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="4839e-188">passcodeRequired</span></span>|<span data-ttu-id="4839e-189">Логический</span><span class="sxs-lookup"><span data-stu-id="4839e-189">Boolean</span></span>|<span data-ttu-id="4839e-190">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="4839e-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="4839e-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4839e-191">osMinimumVersion</span></span>|<span data-ttu-id="4839e-192">String</span><span class="sxs-lookup"><span data-stu-id="4839e-192">String</span></span>|<span data-ttu-id="4839e-193">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="4839e-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="4839e-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4839e-194">osMaximumVersion</span></span>|<span data-ttu-id="4839e-195">String</span><span class="sxs-lookup"><span data-stu-id="4839e-195">String</span></span>|<span data-ttu-id="4839e-196">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="4839e-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="4839e-197">Осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="4839e-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="4839e-198">String</span><span class="sxs-lookup"><span data-stu-id="4839e-198">String</span></span>|<span data-ttu-id="4839e-199">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="4839e-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="4839e-200">Осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="4839e-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="4839e-201">String</span><span class="sxs-lookup"><span data-stu-id="4839e-201">String</span></span>|<span data-ttu-id="4839e-202">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="4839e-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="4839e-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4839e-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4839e-204">Логический</span><span class="sxs-lookup"><span data-stu-id="4839e-204">Boolean</span></span>|<span data-ttu-id="4839e-205">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="4839e-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4839e-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4839e-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4839e-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="4839e-207">Boolean</span></span>|<span data-ttu-id="4839e-208">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="4839e-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="4839e-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4839e-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4839e-210">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="4839e-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4839e-211">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="4839e-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4839e-212">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4839e-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4839e-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="4839e-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="4839e-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="4839e-214">Boolean</span></span>|<span data-ttu-id="4839e-215">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4839e-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="4839e-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="4839e-216">restrictedApps</span></span>|<span data-ttu-id="4839e-217">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4839e-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4839e-218">ПоТребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="4839e-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="4839e-219">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="4839e-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4839e-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="4839e-220">Response</span></span>
<span data-ttu-id="4839e-221">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4839e-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4839e-222">Пример</span><span class="sxs-lookup"><span data-stu-id="4839e-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="4839e-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="4839e-223">Request</span></span>
<span data-ttu-id="4839e-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4839e-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4839e-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="4839e-225">Response</span></span>
<span data-ttu-id="4839e-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4839e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




