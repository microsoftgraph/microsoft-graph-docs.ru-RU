---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ed563d686f2e0a5a3526dc7e3eec1629e18cd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975380"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="09a37-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="09a37-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="09a37-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09a37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09a37-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09a37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09a37-106">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09a37-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="09a37-107">Prerequisites</span></span>
<span data-ttu-id="09a37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09a37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09a37-110">Permission type</span></span>|<span data-ttu-id="09a37-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09a37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09a37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09a37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09a37-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09a37-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09a37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09a37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09a37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09a37-115">Not supported.</span></span>|
|<span data-ttu-id="09a37-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09a37-116">Application</span></span>|<span data-ttu-id="09a37-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09a37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09a37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09a37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="09a37-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09a37-119">Request headers</span></span>
|<span data-ttu-id="09a37-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09a37-120">Header</span></span>|<span data-ttu-id="09a37-121">Значение</span><span class="sxs-lookup"><span data-stu-id="09a37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09a37-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09a37-122">Authorization</span></span>|<span data-ttu-id="09a37-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09a37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09a37-124">Accept</span><span class="sxs-lookup"><span data-stu-id="09a37-124">Accept</span></span>|<span data-ttu-id="09a37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09a37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a37-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09a37-126">Request body</span></span>
<span data-ttu-id="09a37-127">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09a37-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="09a37-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="09a37-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="09a37-129">Property</span></span>|<span data-ttu-id="09a37-130">Тип</span><span class="sxs-lookup"><span data-stu-id="09a37-130">Type</span></span>|<span data-ttu-id="09a37-131">Описание</span><span class="sxs-lookup"><span data-stu-id="09a37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09a37-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09a37-132">roleScopeTagIds</span></span>|<span data-ttu-id="09a37-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09a37-133">String collection</span></span>|<span data-ttu-id="09a37-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="09a37-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09a37-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-136">id</span><span class="sxs-lookup"><span data-stu-id="09a37-136">id</span></span>|<span data-ttu-id="09a37-137">Строка</span><span class="sxs-lookup"><span data-stu-id="09a37-137">String</span></span>|<span data-ttu-id="09a37-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09a37-138">Key of the entity.</span></span> <span data-ttu-id="09a37-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09a37-140">createdDateTime</span></span>|<span data-ttu-id="09a37-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09a37-141">DateTimeOffset</span></span>|<span data-ttu-id="09a37-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="09a37-142">DateTime the object was created.</span></span> <span data-ttu-id="09a37-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-144">description</span><span class="sxs-lookup"><span data-stu-id="09a37-144">description</span></span>|<span data-ttu-id="09a37-145">String</span><span class="sxs-lookup"><span data-stu-id="09a37-145">String</span></span>|<span data-ttu-id="09a37-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09a37-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09a37-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09a37-148">lastModifiedDateTime</span></span>|<span data-ttu-id="09a37-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09a37-149">DateTimeOffset</span></span>|<span data-ttu-id="09a37-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="09a37-150">DateTime the object was last modified.</span></span> <span data-ttu-id="09a37-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-152">displayName</span><span class="sxs-lookup"><span data-stu-id="09a37-152">displayName</span></span>|<span data-ttu-id="09a37-153">Строка</span><span class="sxs-lookup"><span data-stu-id="09a37-153">String</span></span>|<span data-ttu-id="09a37-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09a37-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09a37-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09a37-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-156">version</span><span class="sxs-lookup"><span data-stu-id="09a37-156">version</span></span>|<span data-ttu-id="09a37-157">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-157">Int32</span></span>|<span data-ttu-id="09a37-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09a37-158">Version of the device configuration.</span></span> <span data-ttu-id="09a37-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09a37-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="09a37-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="09a37-160">passcodeBlockSimple</span></span>|<span data-ttu-id="09a37-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a37-161">Boolean</span></span>|<span data-ttu-id="09a37-162">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="09a37-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="09a37-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="09a37-163">passcodeExpirationDays</span></span>|<span data-ttu-id="09a37-164">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-164">Int32</span></span>|<span data-ttu-id="09a37-165">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="09a37-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="09a37-166">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="09a37-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="09a37-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="09a37-167">passcodeMinimumLength</span></span>|<span data-ttu-id="09a37-168">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-168">Int32</span></span>|<span data-ttu-id="09a37-169">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="09a37-169">Minimum length of passcode.</span></span> <span data-ttu-id="09a37-170">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="09a37-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="09a37-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="09a37-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="09a37-172">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-172">Int32</span></span>|<span data-ttu-id="09a37-173">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="09a37-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="09a37-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="09a37-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="09a37-175">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-175">Int32</span></span>|<span data-ttu-id="09a37-176">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="09a37-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="09a37-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="09a37-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="09a37-178">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-178">Int32</span></span>|<span data-ttu-id="09a37-179">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="09a37-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="09a37-180">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="09a37-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="09a37-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="09a37-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="09a37-182">Int32</span><span class="sxs-lookup"><span data-stu-id="09a37-182">Int32</span></span>|<span data-ttu-id="09a37-183">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="09a37-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="09a37-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="09a37-184">passcodeRequiredType</span></span>|[<span data-ttu-id="09a37-185">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="09a37-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="09a37-186">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="09a37-186">The required passcode type.</span></span> <span data-ttu-id="09a37-187">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="09a37-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="09a37-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="09a37-188">passcodeRequired</span></span>|<span data-ttu-id="09a37-189">Логический</span><span class="sxs-lookup"><span data-stu-id="09a37-189">Boolean</span></span>|<span data-ttu-id="09a37-190">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="09a37-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="09a37-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="09a37-191">osMinimumVersion</span></span>|<span data-ttu-id="09a37-192">String</span><span class="sxs-lookup"><span data-stu-id="09a37-192">String</span></span>|<span data-ttu-id="09a37-193">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="09a37-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="09a37-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="09a37-194">osMaximumVersion</span></span>|<span data-ttu-id="09a37-195">String</span><span class="sxs-lookup"><span data-stu-id="09a37-195">String</span></span>|<span data-ttu-id="09a37-196">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="09a37-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="09a37-197">Осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="09a37-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="09a37-198">String</span><span class="sxs-lookup"><span data-stu-id="09a37-198">String</span></span>|<span data-ttu-id="09a37-199">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="09a37-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="09a37-200">Осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="09a37-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="09a37-201">String</span><span class="sxs-lookup"><span data-stu-id="09a37-201">String</span></span>|<span data-ttu-id="09a37-202">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="09a37-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="09a37-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="09a37-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="09a37-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a37-204">Boolean</span></span>|<span data-ttu-id="09a37-205">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="09a37-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="09a37-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="09a37-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="09a37-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a37-207">Boolean</span></span>|<span data-ttu-id="09a37-208">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="09a37-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="09a37-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="09a37-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="09a37-210">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="09a37-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="09a37-211">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="09a37-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="09a37-212">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="09a37-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="09a37-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="09a37-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="09a37-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a37-214">Boolean</span></span>|<span data-ttu-id="09a37-215">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09a37-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="09a37-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="09a37-216">restrictedApps</span></span>|<span data-ttu-id="09a37-217">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="09a37-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="09a37-218">ПоТребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="09a37-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="09a37-219">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="09a37-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="09a37-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="09a37-220">Response</span></span>
<span data-ttu-id="09a37-221">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="09a37-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09a37-222">Пример</span><span class="sxs-lookup"><span data-stu-id="09a37-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="09a37-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="09a37-223">Request</span></span>
<span data-ttu-id="09a37-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09a37-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09a37-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="09a37-225">Response</span></span>
<span data-ttu-id="09a37-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09a37-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




