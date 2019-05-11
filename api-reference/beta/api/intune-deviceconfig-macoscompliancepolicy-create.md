---
title: Create macOSCompliancePolicy
description: Создание объекта macOSCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72c5a81911edd3f82689919b7e1161d354073c05
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923001"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="762a7-103">Create macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="762a7-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="762a7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="762a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="762a7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="762a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="762a7-106">Создание объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="762a7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="762a7-107">Prerequisites</span></span>
<span data-ttu-id="762a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="762a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="762a7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="762a7-110">Permission type</span></span>|<span data-ttu-id="762a7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="762a7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="762a7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="762a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="762a7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="762a7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="762a7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="762a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="762a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="762a7-115">Not supported.</span></span>|
|<span data-ttu-id="762a7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="762a7-116">Application</span></span>|<span data-ttu-id="762a7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="762a7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="762a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="762a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="762a7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="762a7-119">Request headers</span></span>
|<span data-ttu-id="762a7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="762a7-120">Header</span></span>|<span data-ttu-id="762a7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="762a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="762a7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="762a7-122">Authorization</span></span>|<span data-ttu-id="762a7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="762a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="762a7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="762a7-124">Accept</span></span>|<span data-ttu-id="762a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="762a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="762a7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="762a7-126">Request body</span></span>
<span data-ttu-id="762a7-127">В теле запроса добавьте представление объекта macOSCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="762a7-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="762a7-128">Ниже показаны свойства, которые необходимо указывать при создании объекта macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="762a7-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="762a7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="762a7-129">Property</span></span>|<span data-ttu-id="762a7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="762a7-130">Type</span></span>|<span data-ttu-id="762a7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="762a7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="762a7-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="762a7-132">roleScopeTagIds</span></span>|<span data-ttu-id="762a7-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="762a7-133">String collection</span></span>|<span data-ttu-id="762a7-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="762a7-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="762a7-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-136">id</span><span class="sxs-lookup"><span data-stu-id="762a7-136">id</span></span>|<span data-ttu-id="762a7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="762a7-137">String</span></span>|<span data-ttu-id="762a7-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="762a7-138">Key of the entity.</span></span> <span data-ttu-id="762a7-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="762a7-140">createdDateTime</span></span>|<span data-ttu-id="762a7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="762a7-141">DateTimeOffset</span></span>|<span data-ttu-id="762a7-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="762a7-142">DateTime the object was created.</span></span> <span data-ttu-id="762a7-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-144">description</span><span class="sxs-lookup"><span data-stu-id="762a7-144">description</span></span>|<span data-ttu-id="762a7-145">String</span><span class="sxs-lookup"><span data-stu-id="762a7-145">String</span></span>|<span data-ttu-id="762a7-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="762a7-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="762a7-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="762a7-148">lastModifiedDateTime</span></span>|<span data-ttu-id="762a7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="762a7-149">DateTimeOffset</span></span>|<span data-ttu-id="762a7-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="762a7-150">DateTime the object was last modified.</span></span> <span data-ttu-id="762a7-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-152">displayName</span><span class="sxs-lookup"><span data-stu-id="762a7-152">displayName</span></span>|<span data-ttu-id="762a7-153">Строка</span><span class="sxs-lookup"><span data-stu-id="762a7-153">String</span></span>|<span data-ttu-id="762a7-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="762a7-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="762a7-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-156">version</span><span class="sxs-lookup"><span data-stu-id="762a7-156">version</span></span>|<span data-ttu-id="762a7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="762a7-157">Int32</span></span>|<span data-ttu-id="762a7-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="762a7-158">Version of the device configuration.</span></span> <span data-ttu-id="762a7-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="762a7-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="762a7-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="762a7-160">passwordRequired</span></span>|<span data-ttu-id="762a7-161">Логический</span><span class="sxs-lookup"><span data-stu-id="762a7-161">Boolean</span></span>|<span data-ttu-id="762a7-162">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="762a7-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="762a7-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="762a7-163">passwordBlockSimple</span></span>|<span data-ttu-id="762a7-164">Логический</span><span class="sxs-lookup"><span data-stu-id="762a7-164">Boolean</span></span>|<span data-ttu-id="762a7-165">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="762a7-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="762a7-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="762a7-166">passwordExpirationDays</span></span>|<span data-ttu-id="762a7-167">Int32</span><span class="sxs-lookup"><span data-stu-id="762a7-167">Int32</span></span>|<span data-ttu-id="762a7-168">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="762a7-168">Number of days before the password expires.</span></span> <span data-ttu-id="762a7-169">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="762a7-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="762a7-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="762a7-170">passwordMinimumLength</span></span>|<span data-ttu-id="762a7-171">Int32</span><span class="sxs-lookup"><span data-stu-id="762a7-171">Int32</span></span>|<span data-ttu-id="762a7-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="762a7-172">Minimum length of password.</span></span> <span data-ttu-id="762a7-173">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="762a7-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="762a7-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="762a7-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="762a7-175">Int32</span><span class="sxs-lookup"><span data-stu-id="762a7-175">Int32</span></span>|<span data-ttu-id="762a7-176">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="762a7-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="762a7-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="762a7-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="762a7-178">Int32</span><span class="sxs-lookup"><span data-stu-id="762a7-178">Int32</span></span>|<span data-ttu-id="762a7-179">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="762a7-179">Number of previous passwords to block.</span></span> <span data-ttu-id="762a7-180">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="762a7-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="762a7-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="762a7-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="762a7-182">Int32</span><span class="sxs-lookup"><span data-stu-id="762a7-182">Int32</span></span>|<span data-ttu-id="762a7-183">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="762a7-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="762a7-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="762a7-184">passwordRequiredType</span></span>|[<span data-ttu-id="762a7-185">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="762a7-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="762a7-186">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="762a7-186">The required password type.</span></span> <span data-ttu-id="762a7-187">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="762a7-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="762a7-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="762a7-188">osMinimumVersion</span></span>|<span data-ttu-id="762a7-189">Строка</span><span class="sxs-lookup"><span data-stu-id="762a7-189">String</span></span>|<span data-ttu-id="762a7-190">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="762a7-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="762a7-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="762a7-191">osMaximumVersion</span></span>|<span data-ttu-id="762a7-192">String</span><span class="sxs-lookup"><span data-stu-id="762a7-192">String</span></span>|<span data-ttu-id="762a7-193">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="762a7-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="762a7-194">Осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="762a7-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="762a7-195">Строка</span><span class="sxs-lookup"><span data-stu-id="762a7-195">String</span></span>|<span data-ttu-id="762a7-196">Минимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="762a7-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="762a7-197">Осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="762a7-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="762a7-198">Строка</span><span class="sxs-lookup"><span data-stu-id="762a7-198">String</span></span>|<span data-ttu-id="762a7-199">Максимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="762a7-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="762a7-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="762a7-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="762a7-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="762a7-201">Boolean</span></span>|<span data-ttu-id="762a7-202">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="762a7-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="762a7-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="762a7-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="762a7-204">Логический</span><span class="sxs-lookup"><span data-stu-id="762a7-204">Boolean</span></span>|<span data-ttu-id="762a7-205">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="762a7-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="762a7-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="762a7-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="762a7-207">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="762a7-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="762a7-208">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="762a7-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="762a7-209">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="762a7-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="762a7-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="762a7-210">storageRequireEncryption</span></span>|<span data-ttu-id="762a7-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="762a7-211">Boolean</span></span>|<span data-ttu-id="762a7-212">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="762a7-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="762a7-213">Гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="762a7-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="762a7-214">Макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="762a7-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="762a7-215">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="762a7-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="762a7-216">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="762a7-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="762a7-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="762a7-217">firewallEnabled</span></span>|<span data-ttu-id="762a7-218">Логический</span><span class="sxs-lookup"><span data-stu-id="762a7-218">Boolean</span></span>|<span data-ttu-id="762a7-219">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="762a7-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="762a7-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="762a7-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="762a7-221">Логический</span><span class="sxs-lookup"><span data-stu-id="762a7-221">Boolean</span></span>|<span data-ttu-id="762a7-222">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="762a7-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="762a7-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="762a7-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="762a7-224">Логический</span><span class="sxs-lookup"><span data-stu-id="762a7-224">Boolean</span></span>|<span data-ttu-id="762a7-225">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="762a7-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="762a7-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="762a7-226">Response</span></span>
<span data-ttu-id="762a7-227">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="762a7-227">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="762a7-228">Пример</span><span class="sxs-lookup"><span data-stu-id="762a7-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="762a7-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="762a7-229">Request</span></span>
<span data-ttu-id="762a7-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="762a7-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="762a7-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="762a7-231">Response</span></span>
<span data-ttu-id="762a7-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="762a7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




