---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03f8f542b65c4af370bb1e00a86880ffbeae5f95
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442938"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="6b190-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6b190-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="6b190-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6b190-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b190-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b190-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b190-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b190-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b190-107">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b190-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6b190-108">Prerequisites</span></span>
<span data-ttu-id="6b190-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b190-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b190-111">Permission type</span></span>|<span data-ttu-id="6b190-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b190-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b190-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b190-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b190-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b190-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b190-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b190-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b190-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b190-116">Not supported.</span></span>|
|<span data-ttu-id="6b190-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b190-117">Application</span></span>|<span data-ttu-id="6b190-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b190-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b190-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b190-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6b190-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6b190-120">Request headers</span></span>
|<span data-ttu-id="6b190-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b190-121">Header</span></span>|<span data-ttu-id="6b190-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6b190-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b190-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b190-123">Authorization</span></span>|<span data-ttu-id="6b190-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b190-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b190-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6b190-125">Accept</span></span>|<span data-ttu-id="6b190-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b190-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b190-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b190-127">Request body</span></span>
<span data-ttu-id="6b190-128">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b190-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6b190-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="6b190-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b190-130">Property</span></span>|<span data-ttu-id="6b190-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6b190-131">Type</span></span>|<span data-ttu-id="6b190-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6b190-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b190-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b190-133">roleScopeTagIds</span></span>|<span data-ttu-id="6b190-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6b190-134">String collection</span></span>|<span data-ttu-id="6b190-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6b190-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b190-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-137">id</span><span class="sxs-lookup"><span data-stu-id="6b190-137">id</span></span>|<span data-ttu-id="6b190-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6b190-138">String</span></span>|<span data-ttu-id="6b190-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6b190-139">Key of the entity.</span></span> <span data-ttu-id="6b190-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b190-141">createdDateTime</span></span>|<span data-ttu-id="6b190-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b190-142">DateTimeOffset</span></span>|<span data-ttu-id="6b190-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6b190-143">DateTime the object was created.</span></span> <span data-ttu-id="6b190-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-145">description</span><span class="sxs-lookup"><span data-stu-id="6b190-145">description</span></span>|<span data-ttu-id="6b190-146">String</span><span class="sxs-lookup"><span data-stu-id="6b190-146">String</span></span>|<span data-ttu-id="6b190-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b190-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b190-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b190-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6b190-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b190-150">DateTimeOffset</span></span>|<span data-ttu-id="6b190-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6b190-151">DateTime the object was last modified.</span></span> <span data-ttu-id="6b190-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6b190-153">displayName</span></span>|<span data-ttu-id="6b190-154">Строка</span><span class="sxs-lookup"><span data-stu-id="6b190-154">String</span></span>|<span data-ttu-id="6b190-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b190-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b190-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6b190-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-157">version</span><span class="sxs-lookup"><span data-stu-id="6b190-157">version</span></span>|<span data-ttu-id="6b190-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-158">Int32</span></span>|<span data-ttu-id="6b190-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b190-159">Version of the device configuration.</span></span> <span data-ttu-id="6b190-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6b190-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b190-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6b190-161">passcodeBlockSimple</span></span>|<span data-ttu-id="6b190-162">Логический</span><span class="sxs-lookup"><span data-stu-id="6b190-162">Boolean</span></span>|<span data-ttu-id="6b190-163">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="6b190-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6b190-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6b190-164">passcodeExpirationDays</span></span>|<span data-ttu-id="6b190-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-165">Int32</span></span>|<span data-ttu-id="6b190-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6b190-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="6b190-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="6b190-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b190-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6b190-168">passcodeMinimumLength</span></span>|<span data-ttu-id="6b190-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-169">Int32</span></span>|<span data-ttu-id="6b190-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6b190-170">Minimum length of passcode.</span></span> <span data-ttu-id="6b190-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="6b190-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6b190-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6b190-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6b190-173">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-173">Int32</span></span>|<span data-ttu-id="6b190-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="6b190-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6b190-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6b190-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6b190-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-176">Int32</span></span>|<span data-ttu-id="6b190-177">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6b190-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6b190-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6b190-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6b190-179">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-179">Int32</span></span>|<span data-ttu-id="6b190-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="6b190-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="6b190-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6b190-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6b190-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6b190-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6b190-183">Int32</span><span class="sxs-lookup"><span data-stu-id="6b190-183">Int32</span></span>|<span data-ttu-id="6b190-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="6b190-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6b190-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6b190-185">passcodeRequiredType</span></span>|[<span data-ttu-id="6b190-186">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6b190-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6b190-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6b190-187">The required passcode type.</span></span> <span data-ttu-id="6b190-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6b190-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6b190-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6b190-189">passcodeRequired</span></span>|<span data-ttu-id="6b190-190">Логический</span><span class="sxs-lookup"><span data-stu-id="6b190-190">Boolean</span></span>|<span data-ttu-id="6b190-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="6b190-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6b190-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6b190-192">osMinimumVersion</span></span>|<span data-ttu-id="6b190-193">String</span><span class="sxs-lookup"><span data-stu-id="6b190-193">String</span></span>|<span data-ttu-id="6b190-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="6b190-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="6b190-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6b190-195">osMaximumVersion</span></span>|<span data-ttu-id="6b190-196">String</span><span class="sxs-lookup"><span data-stu-id="6b190-196">String</span></span>|<span data-ttu-id="6b190-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="6b190-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="6b190-198">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="6b190-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="6b190-199">String</span><span class="sxs-lookup"><span data-stu-id="6b190-199">String</span></span>|<span data-ttu-id="6b190-200">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="6b190-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="6b190-201">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="6b190-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="6b190-202">String</span><span class="sxs-lookup"><span data-stu-id="6b190-202">String</span></span>|<span data-ttu-id="6b190-203">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="6b190-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="6b190-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6b190-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6b190-205">Логический</span><span class="sxs-lookup"><span data-stu-id="6b190-205">Boolean</span></span>|<span data-ttu-id="6b190-206">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="6b190-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6b190-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6b190-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6b190-208">Логический</span><span class="sxs-lookup"><span data-stu-id="6b190-208">Boolean</span></span>|<span data-ttu-id="6b190-209">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6b190-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="6b190-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6b190-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6b190-211">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="6b190-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6b190-212">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="6b190-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6b190-213">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6b190-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6b190-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="6b190-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="6b190-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b190-215">Boolean</span></span>|<span data-ttu-id="6b190-216">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6b190-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="6b190-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="6b190-217">restrictedApps</span></span>|<span data-ttu-id="6b190-218">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b190-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6b190-219">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="6b190-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="6b190-220">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="6b190-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6b190-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b190-221">Response</span></span>
<span data-ttu-id="6b190-222">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6b190-222">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b190-223">Пример</span><span class="sxs-lookup"><span data-stu-id="6b190-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b190-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b190-224">Request</span></span>
<span data-ttu-id="6b190-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b190-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b190-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b190-226">Response</span></span>
<span data-ttu-id="6b190-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b190-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





