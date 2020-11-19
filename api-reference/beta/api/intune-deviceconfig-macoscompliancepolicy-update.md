---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 31b7de5cc1f3d1cda700c5877d5f7fec7c55174c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297422"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="ee6ca-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ee6ca-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="ee6ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee6ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee6ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee6ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee6ca-107">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee6ca-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ee6ca-108">Prerequisites</span></span>
<span data-ttu-id="ee6ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee6ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee6ca-111">Permission type</span></span>|<span data-ttu-id="ee6ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee6ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee6ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee6ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee6ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee6ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee6ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee6ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee6ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-116">Not supported.</span></span>|
|<span data-ttu-id="ee6ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee6ca-117">Application</span></span>|<span data-ttu-id="ee6ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee6ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee6ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee6ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ee6ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ee6ca-120">Request headers</span></span>
|<span data-ttu-id="ee6ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee6ca-121">Header</span></span>|<span data-ttu-id="ee6ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee6ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee6ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee6ca-123">Authorization</span></span>|<span data-ttu-id="ee6ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee6ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee6ca-125">Accept</span></span>|<span data-ttu-id="ee6ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee6ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee6ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee6ca-127">Request body</span></span>
<span data-ttu-id="ee6ca-128">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="ee6ca-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="ee6ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee6ca-130">Property</span></span>|<span data-ttu-id="ee6ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee6ca-131">Type</span></span>|<span data-ttu-id="ee6ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee6ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee6ca-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee6ca-133">roleScopeTagIds</span></span>|<span data-ttu-id="ee6ca-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ee6ca-134">String collection</span></span>|<span data-ttu-id="ee6ca-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee6ca-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-137">id</span><span class="sxs-lookup"><span data-stu-id="ee6ca-137">id</span></span>|<span data-ttu-id="ee6ca-138">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-138">String</span></span>|<span data-ttu-id="ee6ca-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-139">Key of the entity.</span></span> <span data-ttu-id="ee6ca-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee6ca-141">createdDateTime</span></span>|<span data-ttu-id="ee6ca-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee6ca-142">DateTimeOffset</span></span>|<span data-ttu-id="ee6ca-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-143">DateTime the object was created.</span></span> <span data-ttu-id="ee6ca-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-145">description</span><span class="sxs-lookup"><span data-stu-id="ee6ca-145">description</span></span>|<span data-ttu-id="ee6ca-146">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-146">String</span></span>|<span data-ttu-id="ee6ca-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee6ca-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee6ca-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ee6ca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee6ca-150">DateTimeOffset</span></span>|<span data-ttu-id="ee6ca-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-151">DateTime the object was last modified.</span></span> <span data-ttu-id="ee6ca-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ee6ca-153">displayName</span></span>|<span data-ttu-id="ee6ca-154">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-154">String</span></span>|<span data-ttu-id="ee6ca-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee6ca-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-157">version</span><span class="sxs-lookup"><span data-stu-id="ee6ca-157">version</span></span>|<span data-ttu-id="ee6ca-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ee6ca-158">Int32</span></span>|<span data-ttu-id="ee6ca-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-159">Version of the device configuration.</span></span> <span data-ttu-id="ee6ca-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ee6ca-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee6ca-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ee6ca-161">passwordRequired</span></span>|<span data-ttu-id="ee6ca-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-162">Boolean</span></span>|<span data-ttu-id="ee6ca-163">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="ee6ca-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ee6ca-164">passwordBlockSimple</span></span>|<span data-ttu-id="ee6ca-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-165">Boolean</span></span>|<span data-ttu-id="ee6ca-166">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="ee6ca-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ee6ca-167">passwordExpirationDays</span></span>|<span data-ttu-id="ee6ca-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ee6ca-168">Int32</span></span>|<span data-ttu-id="ee6ca-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-169">Number of days before the password expires.</span></span> <span data-ttu-id="ee6ca-170">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ee6ca-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ee6ca-171">passwordMinimumLength</span></span>|<span data-ttu-id="ee6ca-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ee6ca-172">Int32</span></span>|<span data-ttu-id="ee6ca-173">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-173">Minimum length of password.</span></span> <span data-ttu-id="ee6ca-174">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ee6ca-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ee6ca-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ee6ca-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ee6ca-176">Int32</span></span>|<span data-ttu-id="ee6ca-177">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ee6ca-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ee6ca-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ee6ca-179">Int32</span><span class="sxs-lookup"><span data-stu-id="ee6ca-179">Int32</span></span>|<span data-ttu-id="ee6ca-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-180">Number of previous passwords to block.</span></span> <span data-ttu-id="ee6ca-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ee6ca-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ee6ca-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ee6ca-183">Int32</span><span class="sxs-lookup"><span data-stu-id="ee6ca-183">Int32</span></span>|<span data-ttu-id="ee6ca-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ee6ca-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ee6ca-185">passwordRequiredType</span></span>|[<span data-ttu-id="ee6ca-186">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="ee6ca-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ee6ca-187">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-187">The required password type.</span></span> <span data-ttu-id="ee6ca-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ee6ca-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ee6ca-189">osMinimumVersion</span></span>|<span data-ttu-id="ee6ca-190">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-190">String</span></span>|<span data-ttu-id="ee6ca-191">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="ee6ca-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ee6ca-192">osMaximumVersion</span></span>|<span data-ttu-id="ee6ca-193">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-193">String</span></span>|<span data-ttu-id="ee6ca-194">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="ee6ca-195">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="ee6ca-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="ee6ca-196">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-196">String</span></span>|<span data-ttu-id="ee6ca-197">Минимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="ee6ca-198">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="ee6ca-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="ee6ca-199">String</span><span class="sxs-lookup"><span data-stu-id="ee6ca-199">String</span></span>|<span data-ttu-id="ee6ca-200">Максимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="ee6ca-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ee6ca-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="ee6ca-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-202">Boolean</span></span>|<span data-ttu-id="ee6ca-203">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="ee6ca-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ee6ca-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ee6ca-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-205">Boolean</span></span>|<span data-ttu-id="ee6ca-206">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ee6ca-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ee6ca-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ee6ca-208">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="ee6ca-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ee6ca-209">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ee6ca-210">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ee6ca-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ee6ca-211">storageRequireEncryption</span></span>|<span data-ttu-id="ee6ca-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-212">Boolean</span></span>|<span data-ttu-id="ee6ca-213">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="ee6ca-214">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="ee6ca-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="ee6ca-215">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="ee6ca-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="ee6ca-216">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="ee6ca-217">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="ee6ca-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="ee6ca-218">firewallEnabled</span></span>|<span data-ttu-id="ee6ca-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-219">Boolean</span></span>|<span data-ttu-id="ee6ca-220">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="ee6ca-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="ee6ca-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="ee6ca-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-222">Boolean</span></span>|<span data-ttu-id="ee6ca-223">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="ee6ca-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="ee6ca-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="ee6ca-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="ee6ca-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee6ca-225">Boolean</span></span>|<span data-ttu-id="ee6ca-226">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="ee6ca-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="ee6ca-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee6ca-227">Response</span></span>
<span data-ttu-id="ee6ca-228">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-228">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee6ca-229">Пример</span><span class="sxs-lookup"><span data-stu-id="ee6ca-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee6ca-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee6ca-230">Request</span></span>
<span data-ttu-id="ee6ca-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee6ca-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee6ca-232">Response</span></span>
<span data-ttu-id="ee6ca-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee6ca-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




