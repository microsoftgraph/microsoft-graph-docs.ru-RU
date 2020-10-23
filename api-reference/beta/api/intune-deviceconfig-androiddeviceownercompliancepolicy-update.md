---
title: Обновление Андроиддевицеовнеркомплианцеполици
description: Обновление свойств объекта Андроиддевицеовнеркомплианцеполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4574c8bf63d429a0be8b13af791821770299ea74
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733946"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="44114-103">Обновление Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="44114-103">Update androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="44114-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44114-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44114-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44114-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44114-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44114-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44114-107">Обновление свойств объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="44114-107">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44114-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44114-108">Prerequisites</span></span>
<span data-ttu-id="44114-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44114-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44114-111">Permission type</span></span>|<span data-ttu-id="44114-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44114-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44114-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44114-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44114-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44114-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44114-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44114-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44114-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44114-116">Not supported.</span></span>|
|<span data-ttu-id="44114-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44114-117">Application</span></span>|<span data-ttu-id="44114-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44114-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44114-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44114-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="44114-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44114-120">Request headers</span></span>
|<span data-ttu-id="44114-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44114-121">Header</span></span>|<span data-ttu-id="44114-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44114-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44114-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44114-123">Authorization</span></span>|<span data-ttu-id="44114-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44114-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44114-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44114-125">Accept</span></span>|<span data-ttu-id="44114-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44114-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44114-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44114-127">Request body</span></span>
<span data-ttu-id="44114-128">В тексте запроса добавьте представление объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44114-128">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="44114-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-129">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="44114-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44114-130">Property</span></span>|<span data-ttu-id="44114-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44114-131">Type</span></span>|<span data-ttu-id="44114-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44114-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44114-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44114-133">roleScopeTagIds</span></span>|<span data-ttu-id="44114-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="44114-134">String collection</span></span>|<span data-ttu-id="44114-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="44114-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44114-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-137">id</span><span class="sxs-lookup"><span data-stu-id="44114-137">id</span></span>|<span data-ttu-id="44114-138">Строка</span><span class="sxs-lookup"><span data-stu-id="44114-138">String</span></span>|<span data-ttu-id="44114-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44114-139">Key of the entity.</span></span> <span data-ttu-id="44114-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44114-141">createdDateTime</span></span>|<span data-ttu-id="44114-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44114-142">DateTimeOffset</span></span>|<span data-ttu-id="44114-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="44114-143">DateTime the object was created.</span></span> <span data-ttu-id="44114-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-145">description</span><span class="sxs-lookup"><span data-stu-id="44114-145">description</span></span>|<span data-ttu-id="44114-146">Строка</span><span class="sxs-lookup"><span data-stu-id="44114-146">String</span></span>|<span data-ttu-id="44114-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44114-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44114-149">lastModifiedDateTime</span></span>|<span data-ttu-id="44114-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44114-150">DateTimeOffset</span></span>|<span data-ttu-id="44114-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="44114-151">DateTime the object was last modified.</span></span> <span data-ttu-id="44114-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-153">displayName</span><span class="sxs-lookup"><span data-stu-id="44114-153">displayName</span></span>|<span data-ttu-id="44114-154">Строка</span><span class="sxs-lookup"><span data-stu-id="44114-154">String</span></span>|<span data-ttu-id="44114-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44114-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-157">version</span><span class="sxs-lookup"><span data-stu-id="44114-157">version</span></span>|<span data-ttu-id="44114-158">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-158">Int32</span></span>|<span data-ttu-id="44114-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-159">Version of the device configuration.</span></span> <span data-ttu-id="44114-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44114-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44114-161">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="44114-161">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="44114-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="44114-162">Boolean</span></span>|<span data-ttu-id="44114-163">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="44114-163">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="44114-164">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="44114-164">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="44114-165">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="44114-165">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="44114-166">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="44114-166">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="44114-167">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="44114-167">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="44114-168">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="44114-168">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="44114-169">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="44114-169">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="44114-170">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="44114-170">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="44114-171">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="44114-171">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="44114-172">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="44114-172">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="44114-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="44114-173">Boolean</span></span>|<span data-ttu-id="44114-174">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="44114-174">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="44114-175">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="44114-175">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="44114-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="44114-176">Boolean</span></span>|<span data-ttu-id="44114-177">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="44114-177">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="44114-178">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="44114-178">osMinimumVersion</span></span>|<span data-ttu-id="44114-179">String</span><span class="sxs-lookup"><span data-stu-id="44114-179">String</span></span>|<span data-ttu-id="44114-180">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="44114-180">Minimum Android version.</span></span>|
|<span data-ttu-id="44114-181">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="44114-181">osMaximumVersion</span></span>|<span data-ttu-id="44114-182">String</span><span class="sxs-lookup"><span data-stu-id="44114-182">String</span></span>|<span data-ttu-id="44114-183">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="44114-183">Maximum Android version.</span></span>|
|<span data-ttu-id="44114-184">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="44114-184">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="44114-185">String</span><span class="sxs-lookup"><span data-stu-id="44114-185">String</span></span>|<span data-ttu-id="44114-186">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="44114-186">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="44114-187">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="44114-187">passwordRequired</span></span>|<span data-ttu-id="44114-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="44114-188">Boolean</span></span>|<span data-ttu-id="44114-189">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="44114-189">Require a password to unlock device.</span></span>|
|<span data-ttu-id="44114-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="44114-190">passwordMinimumLength</span></span>|<span data-ttu-id="44114-191">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-191">Int32</span></span>|<span data-ttu-id="44114-192">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="44114-192">Minimum password length.</span></span> <span data-ttu-id="44114-193">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="44114-194">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="44114-194">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="44114-195">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-195">Int32</span></span>|<span data-ttu-id="44114-196">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-196">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="44114-197">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-197">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44114-198">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="44114-198">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="44114-199">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-199">Int32</span></span>|<span data-ttu-id="44114-200">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-200">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="44114-201">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-201">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44114-202">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="44114-202">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="44114-203">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-203">Int32</span></span>|<span data-ttu-id="44114-204">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-204">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="44114-205">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-205">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44114-206">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="44114-206">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="44114-207">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-207">Int32</span></span>|<span data-ttu-id="44114-208">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-208">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="44114-209">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-209">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44114-210">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="44114-210">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="44114-211">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-211">Int32</span></span>|<span data-ttu-id="44114-212">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-212">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="44114-213">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-213">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44114-214">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="44114-214">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="44114-215">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-215">Int32</span></span>|<span data-ttu-id="44114-216">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44114-216">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="44114-217">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44114-217">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44114-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="44114-218">passwordRequiredType</span></span>|[<span data-ttu-id="44114-219">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="44114-219">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="44114-220">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="44114-220">Type of characters in password.</span></span> <span data-ttu-id="44114-221">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="44114-221">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="44114-222">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="44114-222">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="44114-223">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-223">Int32</span></span>|<span data-ttu-id="44114-224">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="44114-224">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="44114-225">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="44114-225">passwordExpirationDays</span></span>|<span data-ttu-id="44114-226">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-226">Int32</span></span>|<span data-ttu-id="44114-227">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="44114-227">Number of days before the password expires.</span></span> <span data-ttu-id="44114-228">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="44114-228">Valid values 1 to 365</span></span>|
|<span data-ttu-id="44114-229">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="44114-229">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="44114-230">Int32</span><span class="sxs-lookup"><span data-stu-id="44114-230">Int32</span></span>|<span data-ttu-id="44114-231">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="44114-231">Number of previous passwords to block.</span></span> <span data-ttu-id="44114-232">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="44114-232">Valid values 1 to 24</span></span>|
|<span data-ttu-id="44114-233">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="44114-233">storageRequireEncryption</span></span>|<span data-ttu-id="44114-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="44114-234">Boolean</span></span>|<span data-ttu-id="44114-235">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="44114-235">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="44114-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="44114-236">Response</span></span>
<span data-ttu-id="44114-237">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44114-237">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44114-238">Пример</span><span class="sxs-lookup"><span data-stu-id="44114-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="44114-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="44114-239">Request</span></span>
<span data-ttu-id="44114-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44114-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44114-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="44114-241">Response</span></span>
<span data-ttu-id="44114-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44114-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





