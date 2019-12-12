---
title: Обновление Андроиддевицеовнеркомплианцеполици
description: Обновление свойств объекта Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7edc69f71a985ee2ec88ce24a8a28516410ee002
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39953896"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="9bf7d-103">Обновление Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="9bf7d-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="9bf7d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bf7d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf7d-106">Обновление свойств объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9bf7d-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf7d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9bf7d-107">Prerequisites</span></span>
<span data-ttu-id="9bf7d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf7d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bf7d-110">Permission type</span></span>|<span data-ttu-id="9bf7d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bf7d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf7d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bf7d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf7d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf7d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bf7d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bf7d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf7d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-115">Not supported.</span></span>|
|<span data-ttu-id="9bf7d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bf7d-116">Application</span></span>|<span data-ttu-id="9bf7d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf7d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bf7d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9bf7d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9bf7d-119">Request headers</span></span>
|<span data-ttu-id="9bf7d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bf7d-120">Header</span></span>|<span data-ttu-id="9bf7d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9bf7d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf7d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bf7d-122">Authorization</span></span>|<span data-ttu-id="9bf7d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf7d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9bf7d-124">Accept</span></span>|<span data-ttu-id="9bf7d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf7d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf7d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9bf7d-126">Request body</span></span>
<span data-ttu-id="9bf7d-127">В тексте запроса добавьте представление объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="9bf7d-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="9bf7d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bf7d-129">Property</span></span>|<span data-ttu-id="9bf7d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9bf7d-130">Type</span></span>|<span data-ttu-id="9bf7d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9bf7d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bf7d-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bf7d-132">roleScopeTagIds</span></span>|<span data-ttu-id="9bf7d-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9bf7d-133">String collection</span></span>|<span data-ttu-id="9bf7d-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9bf7d-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-136">id</span><span class="sxs-lookup"><span data-stu-id="9bf7d-136">id</span></span>|<span data-ttu-id="9bf7d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9bf7d-137">String</span></span>|<span data-ttu-id="9bf7d-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-138">Key of the entity.</span></span> <span data-ttu-id="9bf7d-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf7d-140">createdDateTime</span></span>|<span data-ttu-id="9bf7d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf7d-141">DateTimeOffset</span></span>|<span data-ttu-id="9bf7d-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-142">DateTime the object was created.</span></span> <span data-ttu-id="9bf7d-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-144">description</span><span class="sxs-lookup"><span data-stu-id="9bf7d-144">description</span></span>|<span data-ttu-id="9bf7d-145">String</span><span class="sxs-lookup"><span data-stu-id="9bf7d-145">String</span></span>|<span data-ttu-id="9bf7d-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9bf7d-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf7d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9bf7d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf7d-149">DateTimeOffset</span></span>|<span data-ttu-id="9bf7d-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="9bf7d-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="9bf7d-152">displayName</span></span>|<span data-ttu-id="9bf7d-153">Строка</span><span class="sxs-lookup"><span data-stu-id="9bf7d-153">String</span></span>|<span data-ttu-id="9bf7d-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9bf7d-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-156">version</span><span class="sxs-lookup"><span data-stu-id="9bf7d-156">version</span></span>|<span data-ttu-id="9bf7d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-157">Int32</span></span>|<span data-ttu-id="9bf7d-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-158">Version of the device configuration.</span></span> <span data-ttu-id="9bf7d-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9bf7d-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9bf7d-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9bf7d-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9bf7d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bf7d-161">Boolean</span></span>|<span data-ttu-id="9bf7d-162">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="9bf7d-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9bf7d-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9bf7d-164">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="9bf7d-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9bf7d-165">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9bf7d-166">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9bf7d-167">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="9bf7d-167">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9bf7d-168">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="9bf7d-168">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9bf7d-169">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-169">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9bf7d-170">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-170">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9bf7d-171">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="9bf7d-171">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="9bf7d-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bf7d-172">Boolean</span></span>|<span data-ttu-id="9bf7d-173">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-173">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="9bf7d-174">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="9bf7d-174">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="9bf7d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bf7d-175">Boolean</span></span>|<span data-ttu-id="9bf7d-176">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-176">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="9bf7d-177">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9bf7d-177">osMinimumVersion</span></span>|<span data-ttu-id="9bf7d-178">Строка</span><span class="sxs-lookup"><span data-stu-id="9bf7d-178">String</span></span>|<span data-ttu-id="9bf7d-179">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-179">Minimum Android version.</span></span>|
|<span data-ttu-id="9bf7d-180">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9bf7d-180">osMaximumVersion</span></span>|<span data-ttu-id="9bf7d-181">Строка</span><span class="sxs-lookup"><span data-stu-id="9bf7d-181">String</span></span>|<span data-ttu-id="9bf7d-182">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-182">Maximum Android version.</span></span>|
|<span data-ttu-id="9bf7d-183">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9bf7d-183">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="9bf7d-184">String</span><span class="sxs-lookup"><span data-stu-id="9bf7d-184">String</span></span>|<span data-ttu-id="9bf7d-185">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-185">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="9bf7d-186">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9bf7d-186">passwordRequired</span></span>|<span data-ttu-id="9bf7d-187">Логический</span><span class="sxs-lookup"><span data-stu-id="9bf7d-187">Boolean</span></span>|<span data-ttu-id="9bf7d-188">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-188">Require a password to unlock device.</span></span>|
|<span data-ttu-id="9bf7d-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9bf7d-189">passwordMinimumLength</span></span>|<span data-ttu-id="9bf7d-190">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-190">Int32</span></span>|<span data-ttu-id="9bf7d-191">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-191">Minimum password length.</span></span> <span data-ttu-id="9bf7d-192">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9bf7d-193">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="9bf7d-193">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="9bf7d-194">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-194">Int32</span></span>|<span data-ttu-id="9bf7d-195">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-195">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="9bf7d-196">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9bf7d-197">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="9bf7d-197">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="9bf7d-198">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-198">Int32</span></span>|<span data-ttu-id="9bf7d-199">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-199">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="9bf7d-200">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9bf7d-201">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="9bf7d-201">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="9bf7d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-202">Int32</span></span>|<span data-ttu-id="9bf7d-203">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-203">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="9bf7d-204">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9bf7d-205">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="9bf7d-205">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="9bf7d-206">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-206">Int32</span></span>|<span data-ttu-id="9bf7d-207">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-207">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="9bf7d-208">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9bf7d-209">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="9bf7d-209">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="9bf7d-210">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-210">Int32</span></span>|<span data-ttu-id="9bf7d-211">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-211">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="9bf7d-212">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9bf7d-213">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="9bf7d-213">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="9bf7d-214">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-214">Int32</span></span>|<span data-ttu-id="9bf7d-215">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-215">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="9bf7d-216">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-216">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9bf7d-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9bf7d-217">passwordRequiredType</span></span>|[<span data-ttu-id="9bf7d-218">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="9bf7d-218">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="9bf7d-219">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-219">Type of characters in password.</span></span> <span data-ttu-id="9bf7d-220">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-220">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="9bf7d-221">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9bf7d-221">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9bf7d-222">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-222">Int32</span></span>|<span data-ttu-id="9bf7d-223">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-223">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9bf7d-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9bf7d-224">passwordExpirationDays</span></span>|<span data-ttu-id="9bf7d-225">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-225">Int32</span></span>|<span data-ttu-id="9bf7d-226">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-226">Number of days before the password expires.</span></span> <span data-ttu-id="9bf7d-227">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-227">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9bf7d-228">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="9bf7d-228">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="9bf7d-229">Int32</span><span class="sxs-lookup"><span data-stu-id="9bf7d-229">Int32</span></span>|<span data-ttu-id="9bf7d-230">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-230">Number of previous passwords to block.</span></span> <span data-ttu-id="9bf7d-231">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-231">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9bf7d-232">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9bf7d-232">storageRequireEncryption</span></span>|<span data-ttu-id="9bf7d-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bf7d-233">Boolean</span></span>|<span data-ttu-id="9bf7d-234">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-234">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="9bf7d-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bf7d-235">Response</span></span>
<span data-ttu-id="9bf7d-236">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-236">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf7d-237">Пример</span><span class="sxs-lookup"><span data-stu-id="9bf7d-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf7d-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bf7d-238">Request</span></span>
<span data-ttu-id="9bf7d-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="9bf7d-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bf7d-240">Response</span></span>
<span data-ttu-id="9bf7d-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bf7d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1395

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```





