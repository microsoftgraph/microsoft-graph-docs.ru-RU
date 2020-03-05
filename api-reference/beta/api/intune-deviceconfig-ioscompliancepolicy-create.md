---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ce2abd418d96598f617897c112c36ac70093d3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449056"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="c287f-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c287f-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="c287f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c287f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c287f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c287f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c287f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c287f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c287f-107">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c287f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c287f-108">Prerequisites</span></span>
<span data-ttu-id="c287f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c287f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c287f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c287f-111">Permission type</span></span>|<span data-ttu-id="c287f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c287f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c287f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c287f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c287f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c287f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c287f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c287f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c287f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c287f-116">Not supported.</span></span>|
|<span data-ttu-id="c287f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c287f-117">Application</span></span>|<span data-ttu-id="c287f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c287f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c287f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c287f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c287f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c287f-120">Request headers</span></span>
|<span data-ttu-id="c287f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c287f-121">Header</span></span>|<span data-ttu-id="c287f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c287f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c287f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c287f-123">Authorization</span></span>|<span data-ttu-id="c287f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c287f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c287f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c287f-125">Accept</span></span>|<span data-ttu-id="c287f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c287f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c287f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c287f-127">Request body</span></span>
<span data-ttu-id="c287f-128">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c287f-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="c287f-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c287f-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="c287f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c287f-130">Property</span></span>|<span data-ttu-id="c287f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c287f-131">Type</span></span>|<span data-ttu-id="c287f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c287f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c287f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c287f-133">roleScopeTagIds</span></span>|<span data-ttu-id="c287f-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c287f-134">String collection</span></span>|<span data-ttu-id="c287f-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c287f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c287f-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-137">id</span><span class="sxs-lookup"><span data-stu-id="c287f-137">id</span></span>|<span data-ttu-id="c287f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c287f-138">String</span></span>|<span data-ttu-id="c287f-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c287f-139">Key of the entity.</span></span> <span data-ttu-id="c287f-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c287f-141">createdDateTime</span></span>|<span data-ttu-id="c287f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c287f-142">DateTimeOffset</span></span>|<span data-ttu-id="c287f-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c287f-143">DateTime the object was created.</span></span> <span data-ttu-id="c287f-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-145">description</span><span class="sxs-lookup"><span data-stu-id="c287f-145">description</span></span>|<span data-ttu-id="c287f-146">String</span><span class="sxs-lookup"><span data-stu-id="c287f-146">String</span></span>|<span data-ttu-id="c287f-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c287f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c287f-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c287f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c287f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c287f-150">DateTimeOffset</span></span>|<span data-ttu-id="c287f-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c287f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c287f-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c287f-153">displayName</span></span>|<span data-ttu-id="c287f-154">Строка</span><span class="sxs-lookup"><span data-stu-id="c287f-154">String</span></span>|<span data-ttu-id="c287f-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c287f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c287f-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c287f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-157">version</span><span class="sxs-lookup"><span data-stu-id="c287f-157">version</span></span>|<span data-ttu-id="c287f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-158">Int32</span></span>|<span data-ttu-id="c287f-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c287f-159">Version of the device configuration.</span></span> <span data-ttu-id="c287f-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c287f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c287f-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c287f-161">passcodeBlockSimple</span></span>|<span data-ttu-id="c287f-162">Логический</span><span class="sxs-lookup"><span data-stu-id="c287f-162">Boolean</span></span>|<span data-ttu-id="c287f-163">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="c287f-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="c287f-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c287f-164">passcodeExpirationDays</span></span>|<span data-ttu-id="c287f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-165">Int32</span></span>|<span data-ttu-id="c287f-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="c287f-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="c287f-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="c287f-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c287f-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c287f-168">passcodeMinimumLength</span></span>|<span data-ttu-id="c287f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-169">Int32</span></span>|<span data-ttu-id="c287f-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="c287f-170">Minimum length of passcode.</span></span> <span data-ttu-id="c287f-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="c287f-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c287f-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c287f-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c287f-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-173">Int32</span></span>|<span data-ttu-id="c287f-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="c287f-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="c287f-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c287f-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c287f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-176">Int32</span></span>|<span data-ttu-id="c287f-177">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c287f-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c287f-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="c287f-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="c287f-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-179">Int32</span></span>|<span data-ttu-id="c287f-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="c287f-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="c287f-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="c287f-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c287f-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c287f-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="c287f-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c287f-183">Int32</span></span>|<span data-ttu-id="c287f-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="c287f-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c287f-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="c287f-185">passcodeRequiredType</span></span>|[<span data-ttu-id="c287f-186">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c287f-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c287f-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="c287f-187">The required passcode type.</span></span> <span data-ttu-id="c287f-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c287f-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c287f-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="c287f-189">passcodeRequired</span></span>|<span data-ttu-id="c287f-190">Логический</span><span class="sxs-lookup"><span data-stu-id="c287f-190">Boolean</span></span>|<span data-ttu-id="c287f-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="c287f-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="c287f-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c287f-192">osMinimumVersion</span></span>|<span data-ttu-id="c287f-193">String</span><span class="sxs-lookup"><span data-stu-id="c287f-193">String</span></span>|<span data-ttu-id="c287f-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="c287f-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="c287f-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c287f-195">osMaximumVersion</span></span>|<span data-ttu-id="c287f-196">String</span><span class="sxs-lookup"><span data-stu-id="c287f-196">String</span></span>|<span data-ttu-id="c287f-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="c287f-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="c287f-198">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="c287f-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="c287f-199">String</span><span class="sxs-lookup"><span data-stu-id="c287f-199">String</span></span>|<span data-ttu-id="c287f-200">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="c287f-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="c287f-201">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="c287f-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="c287f-202">String</span><span class="sxs-lookup"><span data-stu-id="c287f-202">String</span></span>|<span data-ttu-id="c287f-203">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="c287f-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="c287f-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c287f-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c287f-205">Логический</span><span class="sxs-lookup"><span data-stu-id="c287f-205">Boolean</span></span>|<span data-ttu-id="c287f-206">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="c287f-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c287f-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c287f-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c287f-208">Логический</span><span class="sxs-lookup"><span data-stu-id="c287f-208">Boolean</span></span>|<span data-ttu-id="c287f-209">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c287f-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="c287f-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c287f-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c287f-211">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c287f-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c287f-212">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c287f-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c287f-213">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c287f-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c287f-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="c287f-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="c287f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c287f-215">Boolean</span></span>|<span data-ttu-id="c287f-216">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c287f-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="c287f-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="c287f-217">restrictedApps</span></span>|<span data-ttu-id="c287f-218">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c287f-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c287f-219">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="c287f-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="c287f-220">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="c287f-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c287f-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="c287f-221">Response</span></span>
<span data-ttu-id="c287f-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c287f-222">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c287f-223">Пример</span><span class="sxs-lookup"><span data-stu-id="c287f-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="c287f-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="c287f-224">Request</span></span>
<span data-ttu-id="c287f-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c287f-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c287f-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="c287f-226">Response</span></span>
<span data-ttu-id="c287f-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c287f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





