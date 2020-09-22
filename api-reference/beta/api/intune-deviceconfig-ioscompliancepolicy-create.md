---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d5d57998519e59cc2e73b7bbd7783610063db24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082751"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="7362a-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7362a-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="7362a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7362a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7362a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7362a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7362a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7362a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7362a-107">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7362a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7362a-108">Prerequisites</span></span>
<span data-ttu-id="7362a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7362a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7362a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7362a-111">Permission type</span></span>|<span data-ttu-id="7362a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7362a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7362a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7362a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7362a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7362a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7362a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7362a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7362a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7362a-116">Not supported.</span></span>|
|<span data-ttu-id="7362a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7362a-117">Application</span></span>|<span data-ttu-id="7362a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7362a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7362a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7362a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7362a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7362a-120">Request headers</span></span>
|<span data-ttu-id="7362a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7362a-121">Header</span></span>|<span data-ttu-id="7362a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7362a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7362a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7362a-123">Authorization</span></span>|<span data-ttu-id="7362a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7362a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7362a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7362a-125">Accept</span></span>|<span data-ttu-id="7362a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7362a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7362a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7362a-127">Request body</span></span>
<span data-ttu-id="7362a-128">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7362a-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="7362a-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7362a-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="7362a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7362a-130">Property</span></span>|<span data-ttu-id="7362a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7362a-131">Type</span></span>|<span data-ttu-id="7362a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7362a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7362a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7362a-133">roleScopeTagIds</span></span>|<span data-ttu-id="7362a-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7362a-134">String collection</span></span>|<span data-ttu-id="7362a-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7362a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7362a-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-137">id</span><span class="sxs-lookup"><span data-stu-id="7362a-137">id</span></span>|<span data-ttu-id="7362a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7362a-138">String</span></span>|<span data-ttu-id="7362a-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7362a-139">Key of the entity.</span></span> <span data-ttu-id="7362a-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7362a-141">createdDateTime</span></span>|<span data-ttu-id="7362a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7362a-142">DateTimeOffset</span></span>|<span data-ttu-id="7362a-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7362a-143">DateTime the object was created.</span></span> <span data-ttu-id="7362a-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-145">description</span><span class="sxs-lookup"><span data-stu-id="7362a-145">description</span></span>|<span data-ttu-id="7362a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="7362a-146">String</span></span>|<span data-ttu-id="7362a-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7362a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7362a-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7362a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7362a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7362a-150">DateTimeOffset</span></span>|<span data-ttu-id="7362a-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7362a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="7362a-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="7362a-153">displayName</span></span>|<span data-ttu-id="7362a-154">Строка</span><span class="sxs-lookup"><span data-stu-id="7362a-154">String</span></span>|<span data-ttu-id="7362a-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7362a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7362a-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-157">version</span><span class="sxs-lookup"><span data-stu-id="7362a-157">version</span></span>|<span data-ttu-id="7362a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-158">Int32</span></span>|<span data-ttu-id="7362a-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7362a-159">Version of the device configuration.</span></span> <span data-ttu-id="7362a-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7362a-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7362a-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7362a-161">passcodeBlockSimple</span></span>|<span data-ttu-id="7362a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7362a-162">Boolean</span></span>|<span data-ttu-id="7362a-163">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="7362a-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="7362a-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7362a-164">passcodeExpirationDays</span></span>|<span data-ttu-id="7362a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-165">Int32</span></span>|<span data-ttu-id="7362a-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="7362a-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="7362a-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="7362a-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="7362a-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7362a-168">passcodeMinimumLength</span></span>|<span data-ttu-id="7362a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-169">Int32</span></span>|<span data-ttu-id="7362a-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="7362a-170">Minimum length of passcode.</span></span> <span data-ttu-id="7362a-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="7362a-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="7362a-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7362a-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7362a-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-173">Int32</span></span>|<span data-ttu-id="7362a-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="7362a-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="7362a-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7362a-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7362a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-176">Int32</span></span>|<span data-ttu-id="7362a-177">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="7362a-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7362a-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="7362a-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="7362a-179">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-179">Int32</span></span>|<span data-ttu-id="7362a-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="7362a-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="7362a-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="7362a-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7362a-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7362a-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="7362a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7362a-183">Int32</span></span>|<span data-ttu-id="7362a-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="7362a-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7362a-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="7362a-185">passcodeRequiredType</span></span>|[<span data-ttu-id="7362a-186">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="7362a-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7362a-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="7362a-187">The required passcode type.</span></span> <span data-ttu-id="7362a-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7362a-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7362a-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="7362a-189">passcodeRequired</span></span>|<span data-ttu-id="7362a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7362a-190">Boolean</span></span>|<span data-ttu-id="7362a-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="7362a-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="7362a-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7362a-192">osMinimumVersion</span></span>|<span data-ttu-id="7362a-193">String</span><span class="sxs-lookup"><span data-stu-id="7362a-193">String</span></span>|<span data-ttu-id="7362a-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="7362a-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="7362a-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7362a-195">osMaximumVersion</span></span>|<span data-ttu-id="7362a-196">String</span><span class="sxs-lookup"><span data-stu-id="7362a-196">String</span></span>|<span data-ttu-id="7362a-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="7362a-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="7362a-198">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="7362a-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="7362a-199">Строка</span><span class="sxs-lookup"><span data-stu-id="7362a-199">String</span></span>|<span data-ttu-id="7362a-200">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="7362a-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="7362a-201">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="7362a-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="7362a-202">Строка</span><span class="sxs-lookup"><span data-stu-id="7362a-202">String</span></span>|<span data-ttu-id="7362a-203">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="7362a-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="7362a-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="7362a-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="7362a-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="7362a-205">Boolean</span></span>|<span data-ttu-id="7362a-206">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="7362a-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="7362a-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7362a-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="7362a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="7362a-208">Boolean</span></span>|<span data-ttu-id="7362a-209">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="7362a-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="7362a-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7362a-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7362a-211">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="7362a-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7362a-212">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="7362a-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7362a-213">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7362a-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7362a-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="7362a-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="7362a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="7362a-215">Boolean</span></span>|<span data-ttu-id="7362a-216">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7362a-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="7362a-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="7362a-217">restrictedApps</span></span>|<span data-ttu-id="7362a-218">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7362a-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7362a-219">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="7362a-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="7362a-220">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="7362a-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7362a-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="7362a-221">Response</span></span>
<span data-ttu-id="7362a-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7362a-222">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7362a-223">Пример</span><span class="sxs-lookup"><span data-stu-id="7362a-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="7362a-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="7362a-224">Request</span></span>
<span data-ttu-id="7362a-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7362a-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="7362a-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="7362a-226">Response</span></span>
<span data-ttu-id="7362a-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7362a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






