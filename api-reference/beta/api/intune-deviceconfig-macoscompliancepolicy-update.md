---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e602da2c22104b94b58689e02b760bb810c0cea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42747702"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="6e8ec-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6e8ec-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="6e8ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e8ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e8ec-106">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e8ec-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8ec-107">Prerequisites</span></span>
<span data-ttu-id="6e8ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e8ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8ec-110">Permission type</span></span>|<span data-ttu-id="6e8ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e8ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e8ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e8ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e8ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e8ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e8ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e8ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e8ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-115">Not supported.</span></span>|
|<span data-ttu-id="6e8ec-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e8ec-116">Application</span></span>|<span data-ttu-id="6e8ec-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e8ec-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e8ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e8ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6e8ec-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e8ec-119">Request headers</span></span>
|<span data-ttu-id="6e8ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e8ec-120">Header</span></span>|<span data-ttu-id="6e8ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6e8ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e8ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e8ec-122">Authorization</span></span>|<span data-ttu-id="6e8ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e8ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6e8ec-124">Accept</span></span>|<span data-ttu-id="6e8ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e8ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e8ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e8ec-126">Request body</span></span>
<span data-ttu-id="6e8ec-127">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6e8ec-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="6e8ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e8ec-129">Property</span></span>|<span data-ttu-id="6e8ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6e8ec-130">Type</span></span>|<span data-ttu-id="6e8ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6e8ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e8ec-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e8ec-132">roleScopeTagIds</span></span>|<span data-ttu-id="6e8ec-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e8ec-133">String collection</span></span>|<span data-ttu-id="6e8ec-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e8ec-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-136">id</span><span class="sxs-lookup"><span data-stu-id="6e8ec-136">id</span></span>|<span data-ttu-id="6e8ec-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6e8ec-137">String</span></span>|<span data-ttu-id="6e8ec-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-138">Key of the entity.</span></span> <span data-ttu-id="6e8ec-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e8ec-140">createdDateTime</span></span>|<span data-ttu-id="6e8ec-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e8ec-141">DateTimeOffset</span></span>|<span data-ttu-id="6e8ec-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-142">DateTime the object was created.</span></span> <span data-ttu-id="6e8ec-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-144">description</span><span class="sxs-lookup"><span data-stu-id="6e8ec-144">description</span></span>|<span data-ttu-id="6e8ec-145">String</span><span class="sxs-lookup"><span data-stu-id="6e8ec-145">String</span></span>|<span data-ttu-id="6e8ec-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e8ec-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e8ec-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6e8ec-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e8ec-149">DateTimeOffset</span></span>|<span data-ttu-id="6e8ec-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6e8ec-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6e8ec-152">displayName</span></span>|<span data-ttu-id="6e8ec-153">Строка</span><span class="sxs-lookup"><span data-stu-id="6e8ec-153">String</span></span>|<span data-ttu-id="6e8ec-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e8ec-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-156">version</span><span class="sxs-lookup"><span data-stu-id="6e8ec-156">version</span></span>|<span data-ttu-id="6e8ec-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ec-157">Int32</span></span>|<span data-ttu-id="6e8ec-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-158">Version of the device configuration.</span></span> <span data-ttu-id="6e8ec-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ec-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e8ec-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6e8ec-160">passwordRequired</span></span>|<span data-ttu-id="6e8ec-161">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ec-161">Boolean</span></span>|<span data-ttu-id="6e8ec-162">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6e8ec-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6e8ec-163">passwordBlockSimple</span></span>|<span data-ttu-id="6e8ec-164">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ec-164">Boolean</span></span>|<span data-ttu-id="6e8ec-165">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="6e8ec-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6e8ec-166">passwordExpirationDays</span></span>|<span data-ttu-id="6e8ec-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ec-167">Int32</span></span>|<span data-ttu-id="6e8ec-168">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-168">Number of days before the password expires.</span></span> <span data-ttu-id="6e8ec-169">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6e8ec-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6e8ec-170">passwordMinimumLength</span></span>|<span data-ttu-id="6e8ec-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ec-171">Int32</span></span>|<span data-ttu-id="6e8ec-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-172">Minimum length of password.</span></span> <span data-ttu-id="6e8ec-173">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6e8ec-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6e8ec-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6e8ec-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ec-175">Int32</span></span>|<span data-ttu-id="6e8ec-176">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6e8ec-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6e8ec-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6e8ec-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ec-178">Int32</span></span>|<span data-ttu-id="6e8ec-179">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-179">Number of previous passwords to block.</span></span> <span data-ttu-id="6e8ec-180">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6e8ec-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6e8ec-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6e8ec-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ec-182">Int32</span></span>|<span data-ttu-id="6e8ec-183">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6e8ec-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6e8ec-184">passwordRequiredType</span></span>|[<span data-ttu-id="6e8ec-185">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6e8ec-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6e8ec-186">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-186">The required password type.</span></span> <span data-ttu-id="6e8ec-187">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6e8ec-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e8ec-188">osMinimumVersion</span></span>|<span data-ttu-id="6e8ec-189">String</span><span class="sxs-lookup"><span data-stu-id="6e8ec-189">String</span></span>|<span data-ttu-id="6e8ec-190">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="6e8ec-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e8ec-191">osMaximumVersion</span></span>|<span data-ttu-id="6e8ec-192">String</span><span class="sxs-lookup"><span data-stu-id="6e8ec-192">String</span></span>|<span data-ttu-id="6e8ec-193">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="6e8ec-194">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="6e8ec-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="6e8ec-195">String</span><span class="sxs-lookup"><span data-stu-id="6e8ec-195">String</span></span>|<span data-ttu-id="6e8ec-196">Минимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="6e8ec-197">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="6e8ec-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="6e8ec-198">String</span><span class="sxs-lookup"><span data-stu-id="6e8ec-198">String</span></span>|<span data-ttu-id="6e8ec-199">Максимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="6e8ec-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e8ec-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="6e8ec-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e8ec-201">Boolean</span></span>|<span data-ttu-id="6e8ec-202">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="6e8ec-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e8ec-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6e8ec-204">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ec-204">Boolean</span></span>|<span data-ttu-id="6e8ec-205">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6e8ec-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6e8ec-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6e8ec-207">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="6e8ec-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6e8ec-208">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6e8ec-209">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6e8ec-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6e8ec-210">storageRequireEncryption</span></span>|<span data-ttu-id="6e8ec-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e8ec-211">Boolean</span></span>|<span data-ttu-id="6e8ec-212">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="6e8ec-213">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="6e8ec-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="6e8ec-214">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="6e8ec-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="6e8ec-215">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="6e8ec-216">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="6e8ec-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="6e8ec-217">firewallEnabled</span></span>|<span data-ttu-id="6e8ec-218">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ec-218">Boolean</span></span>|<span data-ttu-id="6e8ec-219">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="6e8ec-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="6e8ec-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="6e8ec-221">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ec-221">Boolean</span></span>|<span data-ttu-id="6e8ec-222">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="6e8ec-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="6e8ec-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="6e8ec-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="6e8ec-224">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ec-224">Boolean</span></span>|<span data-ttu-id="6e8ec-225">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="6e8ec-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="6e8ec-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e8ec-226">Response</span></span>
<span data-ttu-id="6e8ec-227">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e8ec-228">Пример</span><span class="sxs-lookup"><span data-stu-id="6e8ec-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e8ec-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e8ec-229">Request</span></span>
<span data-ttu-id="6e8ec-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1083

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="6e8ec-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e8ec-231">Response</span></span>
<span data-ttu-id="6e8ec-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e8ec-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```




