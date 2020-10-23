---
title: Create macOSCompliancePolicy
description: Создание объекта macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efbec3d5d89524900ab9c5b597a1fc82a41c9f46
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704401"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="08d24-103">Create macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="08d24-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="08d24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08d24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08d24-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08d24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08d24-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08d24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08d24-107">Создание объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08d24-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="08d24-108">Prerequisites</span></span>
<span data-ttu-id="08d24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08d24-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08d24-111">Permission type</span></span>|<span data-ttu-id="08d24-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08d24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08d24-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08d24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08d24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08d24-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08d24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08d24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08d24-116">Not supported.</span></span>|
|<span data-ttu-id="08d24-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08d24-117">Application</span></span>|<span data-ttu-id="08d24-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d24-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08d24-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08d24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="08d24-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08d24-120">Request headers</span></span>
|<span data-ttu-id="08d24-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08d24-121">Header</span></span>|<span data-ttu-id="08d24-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08d24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08d24-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08d24-123">Authorization</span></span>|<span data-ttu-id="08d24-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08d24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08d24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08d24-125">Accept</span></span>|<span data-ttu-id="08d24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08d24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08d24-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08d24-127">Request body</span></span>
<span data-ttu-id="08d24-128">В теле запроса добавьте представление объекта macOSCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08d24-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="08d24-129">Ниже показаны свойства, которые необходимо указывать при создании объекта macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="08d24-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="08d24-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08d24-130">Property</span></span>|<span data-ttu-id="08d24-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08d24-131">Type</span></span>|<span data-ttu-id="08d24-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08d24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08d24-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08d24-133">roleScopeTagIds</span></span>|<span data-ttu-id="08d24-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08d24-134">String collection</span></span>|<span data-ttu-id="08d24-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="08d24-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08d24-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-137">id</span><span class="sxs-lookup"><span data-stu-id="08d24-137">id</span></span>|<span data-ttu-id="08d24-138">Строка</span><span class="sxs-lookup"><span data-stu-id="08d24-138">String</span></span>|<span data-ttu-id="08d24-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08d24-139">Key of the entity.</span></span> <span data-ttu-id="08d24-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08d24-141">createdDateTime</span></span>|<span data-ttu-id="08d24-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d24-142">DateTimeOffset</span></span>|<span data-ttu-id="08d24-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="08d24-143">DateTime the object was created.</span></span> <span data-ttu-id="08d24-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-145">description</span><span class="sxs-lookup"><span data-stu-id="08d24-145">description</span></span>|<span data-ttu-id="08d24-146">Строка</span><span class="sxs-lookup"><span data-stu-id="08d24-146">String</span></span>|<span data-ttu-id="08d24-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08d24-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08d24-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08d24-149">lastModifiedDateTime</span></span>|<span data-ttu-id="08d24-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d24-150">DateTimeOffset</span></span>|<span data-ttu-id="08d24-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="08d24-151">DateTime the object was last modified.</span></span> <span data-ttu-id="08d24-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-153">displayName</span><span class="sxs-lookup"><span data-stu-id="08d24-153">displayName</span></span>|<span data-ttu-id="08d24-154">Строка</span><span class="sxs-lookup"><span data-stu-id="08d24-154">String</span></span>|<span data-ttu-id="08d24-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08d24-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08d24-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-157">version</span><span class="sxs-lookup"><span data-stu-id="08d24-157">version</span></span>|<span data-ttu-id="08d24-158">Int32</span><span class="sxs-lookup"><span data-stu-id="08d24-158">Int32</span></span>|<span data-ttu-id="08d24-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08d24-159">Version of the device configuration.</span></span> <span data-ttu-id="08d24-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08d24-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08d24-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="08d24-161">passwordRequired</span></span>|<span data-ttu-id="08d24-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d24-162">Boolean</span></span>|<span data-ttu-id="08d24-163">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="08d24-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="08d24-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="08d24-164">passwordBlockSimple</span></span>|<span data-ttu-id="08d24-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d24-165">Boolean</span></span>|<span data-ttu-id="08d24-166">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="08d24-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="08d24-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="08d24-167">passwordExpirationDays</span></span>|<span data-ttu-id="08d24-168">Int32</span><span class="sxs-lookup"><span data-stu-id="08d24-168">Int32</span></span>|<span data-ttu-id="08d24-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="08d24-169">Number of days before the password expires.</span></span> <span data-ttu-id="08d24-170">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="08d24-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="08d24-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="08d24-171">passwordMinimumLength</span></span>|<span data-ttu-id="08d24-172">Int32</span><span class="sxs-lookup"><span data-stu-id="08d24-172">Int32</span></span>|<span data-ttu-id="08d24-173">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="08d24-173">Minimum length of password.</span></span> <span data-ttu-id="08d24-174">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="08d24-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="08d24-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="08d24-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="08d24-176">Int32</span><span class="sxs-lookup"><span data-stu-id="08d24-176">Int32</span></span>|<span data-ttu-id="08d24-177">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="08d24-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="08d24-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="08d24-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="08d24-179">Int32</span><span class="sxs-lookup"><span data-stu-id="08d24-179">Int32</span></span>|<span data-ttu-id="08d24-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="08d24-180">Number of previous passwords to block.</span></span> <span data-ttu-id="08d24-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="08d24-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="08d24-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="08d24-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="08d24-183">Int32</span><span class="sxs-lookup"><span data-stu-id="08d24-183">Int32</span></span>|<span data-ttu-id="08d24-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="08d24-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="08d24-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="08d24-185">passwordRequiredType</span></span>|[<span data-ttu-id="08d24-186">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="08d24-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="08d24-187">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="08d24-187">The required password type.</span></span> <span data-ttu-id="08d24-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="08d24-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="08d24-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="08d24-189">osMinimumVersion</span></span>|<span data-ttu-id="08d24-190">String</span><span class="sxs-lookup"><span data-stu-id="08d24-190">String</span></span>|<span data-ttu-id="08d24-191">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="08d24-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="08d24-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="08d24-192">osMaximumVersion</span></span>|<span data-ttu-id="08d24-193">String</span><span class="sxs-lookup"><span data-stu-id="08d24-193">String</span></span>|<span data-ttu-id="08d24-194">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="08d24-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="08d24-195">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="08d24-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="08d24-196">Строка</span><span class="sxs-lookup"><span data-stu-id="08d24-196">String</span></span>|<span data-ttu-id="08d24-197">Минимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="08d24-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="08d24-198">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="08d24-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="08d24-199">Строка</span><span class="sxs-lookup"><span data-stu-id="08d24-199">String</span></span>|<span data-ttu-id="08d24-200">Максимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="08d24-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="08d24-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="08d24-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="08d24-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d24-202">Boolean</span></span>|<span data-ttu-id="08d24-203">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="08d24-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="08d24-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="08d24-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="08d24-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d24-205">Boolean</span></span>|<span data-ttu-id="08d24-206">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="08d24-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="08d24-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08d24-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="08d24-208">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="08d24-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="08d24-209">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="08d24-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="08d24-210">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="08d24-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="08d24-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="08d24-211">storageRequireEncryption</span></span>|<span data-ttu-id="08d24-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d24-212">Boolean</span></span>|<span data-ttu-id="08d24-213">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="08d24-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="08d24-214">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="08d24-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="08d24-215">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="08d24-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="08d24-216">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="08d24-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="08d24-217">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="08d24-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="08d24-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="08d24-218">firewallEnabled</span></span>|<span data-ttu-id="08d24-219">Логический</span><span class="sxs-lookup"><span data-stu-id="08d24-219">Boolean</span></span>|<span data-ttu-id="08d24-220">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="08d24-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="08d24-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="08d24-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="08d24-222">Логический</span><span class="sxs-lookup"><span data-stu-id="08d24-222">Boolean</span></span>|<span data-ttu-id="08d24-223">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="08d24-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="08d24-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="08d24-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="08d24-225">Логический</span><span class="sxs-lookup"><span data-stu-id="08d24-225">Boolean</span></span>|<span data-ttu-id="08d24-226">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="08d24-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="08d24-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="08d24-227">Response</span></span>
<span data-ttu-id="08d24-228">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08d24-228">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08d24-229">Пример</span><span class="sxs-lookup"><span data-stu-id="08d24-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="08d24-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="08d24-230">Request</span></span>
<span data-ttu-id="08d24-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08d24-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="08d24-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="08d24-232">Response</span></span>
<span data-ttu-id="08d24-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08d24-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





