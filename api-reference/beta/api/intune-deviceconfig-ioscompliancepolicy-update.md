---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a90cc72523685efefb0b203f7d8f73b54c4983cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151489"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="b1830-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b1830-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="b1830-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1830-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1830-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1830-107">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1830-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b1830-108">Prerequisites</span></span>
<span data-ttu-id="b1830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1830-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1830-111">Permission type</span></span>|<span data-ttu-id="b1830-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1830-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1830-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1830-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1830-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1830-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1830-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1830-116">Not supported.</span></span>|
|<span data-ttu-id="b1830-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1830-117">Application</span></span>|<span data-ttu-id="b1830-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1830-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1830-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b1830-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1830-120">Request headers</span></span>
|<span data-ttu-id="b1830-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1830-121">Header</span></span>|<span data-ttu-id="b1830-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1830-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1830-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1830-123">Authorization</span></span>|<span data-ttu-id="b1830-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1830-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1830-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1830-125">Accept</span></span>|<span data-ttu-id="b1830-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1830-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1830-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1830-127">Request body</span></span>
<span data-ttu-id="b1830-128">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1830-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="b1830-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="b1830-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1830-130">Property</span></span>|<span data-ttu-id="b1830-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1830-131">Type</span></span>|<span data-ttu-id="b1830-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1830-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1830-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1830-133">roleScopeTagIds</span></span>|<span data-ttu-id="b1830-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1830-134">String collection</span></span>|<span data-ttu-id="b1830-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="b1830-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1830-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-137">id</span><span class="sxs-lookup"><span data-stu-id="b1830-137">id</span></span>|<span data-ttu-id="b1830-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b1830-138">String</span></span>|<span data-ttu-id="b1830-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1830-139">Key of the entity.</span></span> <span data-ttu-id="b1830-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1830-141">createdDateTime</span></span>|<span data-ttu-id="b1830-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1830-142">DateTimeOffset</span></span>|<span data-ttu-id="b1830-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b1830-143">DateTime the object was created.</span></span> <span data-ttu-id="b1830-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-145">description</span><span class="sxs-lookup"><span data-stu-id="b1830-145">description</span></span>|<span data-ttu-id="b1830-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b1830-146">String</span></span>|<span data-ttu-id="b1830-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1830-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1830-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1830-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b1830-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1830-150">DateTimeOffset</span></span>|<span data-ttu-id="b1830-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b1830-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b1830-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b1830-153">displayName</span></span>|<span data-ttu-id="b1830-154">Строка</span><span class="sxs-lookup"><span data-stu-id="b1830-154">String</span></span>|<span data-ttu-id="b1830-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1830-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1830-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-157">version</span><span class="sxs-lookup"><span data-stu-id="b1830-157">version</span></span>|<span data-ttu-id="b1830-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-158">Int32</span></span>|<span data-ttu-id="b1830-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1830-159">Version of the device configuration.</span></span> <span data-ttu-id="b1830-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1830-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1830-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b1830-161">passcodeBlockSimple</span></span>|<span data-ttu-id="b1830-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1830-162">Boolean</span></span>|<span data-ttu-id="b1830-163">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="b1830-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b1830-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b1830-164">passcodeExpirationDays</span></span>|<span data-ttu-id="b1830-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-165">Int32</span></span>|<span data-ttu-id="b1830-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="b1830-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="b1830-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="b1830-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b1830-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b1830-168">passcodeMinimumLength</span></span>|<span data-ttu-id="b1830-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-169">Int32</span></span>|<span data-ttu-id="b1830-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="b1830-170">Minimum length of passcode.</span></span> <span data-ttu-id="b1830-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="b1830-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b1830-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b1830-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b1830-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-173">Int32</span></span>|<span data-ttu-id="b1830-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="b1830-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b1830-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b1830-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b1830-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-176">Int32</span></span>|<span data-ttu-id="b1830-177">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="b1830-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b1830-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b1830-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b1830-179">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-179">Int32</span></span>|<span data-ttu-id="b1830-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="b1830-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="b1830-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="b1830-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b1830-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b1830-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b1830-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b1830-183">Int32</span></span>|<span data-ttu-id="b1830-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="b1830-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b1830-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b1830-185">passcodeRequiredType</span></span>|[<span data-ttu-id="b1830-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b1830-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b1830-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="b1830-187">The required passcode type.</span></span> <span data-ttu-id="b1830-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b1830-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b1830-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b1830-189">passcodeRequired</span></span>|<span data-ttu-id="b1830-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1830-190">Boolean</span></span>|<span data-ttu-id="b1830-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="b1830-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b1830-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1830-192">osMinimumVersion</span></span>|<span data-ttu-id="b1830-193">String</span><span class="sxs-lookup"><span data-stu-id="b1830-193">String</span></span>|<span data-ttu-id="b1830-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="b1830-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="b1830-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1830-195">osMaximumVersion</span></span>|<span data-ttu-id="b1830-196">String</span><span class="sxs-lookup"><span data-stu-id="b1830-196">String</span></span>|<span data-ttu-id="b1830-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="b1830-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="b1830-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="b1830-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="b1830-199">Строка</span><span class="sxs-lookup"><span data-stu-id="b1830-199">String</span></span>|<span data-ttu-id="b1830-200">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="b1830-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="b1830-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="b1830-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="b1830-202">Строка</span><span class="sxs-lookup"><span data-stu-id="b1830-202">String</span></span>|<span data-ttu-id="b1830-203">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="b1830-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="b1830-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b1830-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b1830-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1830-205">Boolean</span></span>|<span data-ttu-id="b1830-206">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="b1830-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b1830-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1830-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b1830-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1830-208">Boolean</span></span>|<span data-ttu-id="b1830-209">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="b1830-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="b1830-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b1830-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b1830-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b1830-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b1830-212">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="b1830-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b1830-213">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b1830-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b1830-214">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b1830-214">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b1830-215">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b1830-215">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b1830-216">MDATP требует минимального уровня риска для защиты от мобильных угроз, чтобы сообщить о несоблюдении.</span><span class="sxs-lookup"><span data-stu-id="b1830-216">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b1830-217">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b1830-217">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b1830-218">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="b1830-218">managedEmailProfileRequired</span></span>|<span data-ttu-id="b1830-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1830-219">Boolean</span></span>|<span data-ttu-id="b1830-220">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b1830-220">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="b1830-221">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="b1830-221">restrictedApps</span></span>|<span data-ttu-id="b1830-222">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1830-222">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b1830-223">Требуй, чтобы на устройстве не устанавливались указанные приложения.</span><span class="sxs-lookup"><span data-stu-id="b1830-223">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="b1830-224">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="b1830-224">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b1830-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1830-225">Response</span></span>
<span data-ttu-id="b1830-226">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b1830-226">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1830-227">Пример</span><span class="sxs-lookup"><span data-stu-id="b1830-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1830-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1830-228">Request</span></span>
<span data-ttu-id="b1830-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1830-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1304

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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

### <a name="response"></a><span data-ttu-id="b1830-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1830-230">Response</span></span>
<span data-ttu-id="b1830-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1830-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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




