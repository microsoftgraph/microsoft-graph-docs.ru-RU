---
title: Обновление Андроиддевицеовнеркомплианцеполици
description: Обновление свойств объекта Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc10c99329c7efd38f95d9cd41d94cae4e47ab30
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170002"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="e4ea1-103">Обновление Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="e4ea1-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="e4ea1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4ea1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4ea1-106">Обновление свойств объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e4ea1-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4ea1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4ea1-107">Prerequisites</span></span>
<span data-ttu-id="e4ea1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4ea1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4ea1-110">Permission type</span></span>|<span data-ttu-id="e4ea1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4ea1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4ea1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4ea1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4ea1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ea1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4ea1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4ea1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4ea1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-115">Not supported.</span></span>|
|<span data-ttu-id="e4ea1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4ea1-116">Application</span></span>|<span data-ttu-id="e4ea1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ea1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4ea1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4ea1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e4ea1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4ea1-119">Request headers</span></span>
|<span data-ttu-id="e4ea1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4ea1-120">Header</span></span>|<span data-ttu-id="e4ea1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e4ea1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4ea1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4ea1-122">Authorization</span></span>|<span data-ttu-id="e4ea1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4ea1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e4ea1-124">Accept</span></span>|<span data-ttu-id="e4ea1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4ea1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4ea1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4ea1-126">Request body</span></span>
<span data-ttu-id="e4ea1-127">В тексте запроса добавьте представление объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="e4ea1-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="e4ea1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4ea1-129">Property</span></span>|<span data-ttu-id="e4ea1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e4ea1-130">Type</span></span>|<span data-ttu-id="e4ea1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e4ea1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ea1-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4ea1-132">roleScopeTagIds</span></span>|<span data-ttu-id="e4ea1-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e4ea1-133">String collection</span></span>|<span data-ttu-id="e4ea1-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e4ea1-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-136">id</span><span class="sxs-lookup"><span data-stu-id="e4ea1-136">id</span></span>|<span data-ttu-id="e4ea1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ea1-137">String</span></span>|<span data-ttu-id="e4ea1-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-138">Key of the entity.</span></span> <span data-ttu-id="e4ea1-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ea1-140">createdDateTime</span></span>|<span data-ttu-id="e4ea1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ea1-141">DateTimeOffset</span></span>|<span data-ttu-id="e4ea1-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-142">DateTime the object was created.</span></span> <span data-ttu-id="e4ea1-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-144">description</span><span class="sxs-lookup"><span data-stu-id="e4ea1-144">description</span></span>|<span data-ttu-id="e4ea1-145">String</span><span class="sxs-lookup"><span data-stu-id="e4ea1-145">String</span></span>|<span data-ttu-id="e4ea1-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4ea1-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ea1-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e4ea1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ea1-149">DateTimeOffset</span></span>|<span data-ttu-id="e4ea1-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-150">DateTime the object was last modified.</span></span> <span data-ttu-id="e4ea1-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e4ea1-152">displayName</span></span>|<span data-ttu-id="e4ea1-153">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ea1-153">String</span></span>|<span data-ttu-id="e4ea1-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4ea1-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-156">version</span><span class="sxs-lookup"><span data-stu-id="e4ea1-156">version</span></span>|<span data-ttu-id="e4ea1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-157">Int32</span></span>|<span data-ttu-id="e4ea1-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-158">Version of the device configuration.</span></span> <span data-ttu-id="e4ea1-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4ea1-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4ea1-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e4ea1-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e4ea1-161">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-161">Boolean</span></span>|<span data-ttu-id="e4ea1-162">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="e4ea1-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e4ea1-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e4ea1-164">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="e4ea1-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e4ea1-165">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e4ea1-166">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e4ea1-167">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="e4ea1-167">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="e4ea1-168">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-168">Boolean</span></span>|<span data-ttu-id="e4ea1-169">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-169">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="e4ea1-170">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="e4ea1-170">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="e4ea1-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4ea1-171">Boolean</span></span>|<span data-ttu-id="e4ea1-172">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-172">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="e4ea1-173">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e4ea1-173">osMinimumVersion</span></span>|<span data-ttu-id="e4ea1-174">String.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-174">String</span></span>|<span data-ttu-id="e4ea1-175">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-175">Minimum Android version.</span></span>|
|<span data-ttu-id="e4ea1-176">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e4ea1-176">osMaximumVersion</span></span>|<span data-ttu-id="e4ea1-177">String.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-177">String</span></span>|<span data-ttu-id="e4ea1-178">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-178">Maximum Android version.</span></span>|
|<span data-ttu-id="e4ea1-179">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="e4ea1-179">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="e4ea1-180">String</span><span class="sxs-lookup"><span data-stu-id="e4ea1-180">String</span></span>|<span data-ttu-id="e4ea1-181">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-181">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="e4ea1-182">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e4ea1-182">passwordRequired</span></span>|<span data-ttu-id="e4ea1-183">Логический</span><span class="sxs-lookup"><span data-stu-id="e4ea1-183">Boolean</span></span>|<span data-ttu-id="e4ea1-184">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-184">Require a password to unlock device.</span></span>|
|<span data-ttu-id="e4ea1-185">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e4ea1-185">passwordMinimumLength</span></span>|<span data-ttu-id="e4ea1-186">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-186">Int32</span></span>|<span data-ttu-id="e4ea1-187">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-187">Minimum password length.</span></span> <span data-ttu-id="e4ea1-188">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-188">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e4ea1-189">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="e4ea1-189">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="e4ea1-190">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-190">Int32</span></span>|<span data-ttu-id="e4ea1-191">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-191">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="e4ea1-192">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e4ea1-193">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="e4ea1-193">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="e4ea1-194">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-194">Int32</span></span>|<span data-ttu-id="e4ea1-195">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-195">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="e4ea1-196">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e4ea1-197">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="e4ea1-197">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="e4ea1-198">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-198">Int32</span></span>|<span data-ttu-id="e4ea1-199">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-199">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="e4ea1-200">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e4ea1-201">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="e4ea1-201">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="e4ea1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-202">Int32</span></span>|<span data-ttu-id="e4ea1-203">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-203">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="e4ea1-204">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e4ea1-205">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="e4ea1-205">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="e4ea1-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-206">Int32</span></span>|<span data-ttu-id="e4ea1-207">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-207">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="e4ea1-208">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e4ea1-209">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="e4ea1-209">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="e4ea1-210">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-210">Int32</span></span>|<span data-ttu-id="e4ea1-211">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-211">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="e4ea1-212">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e4ea1-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e4ea1-213">passwordRequiredType</span></span>|[<span data-ttu-id="e4ea1-214">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="e4ea1-214">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="e4ea1-215">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-215">Type of characters in password.</span></span> <span data-ttu-id="e4ea1-216">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-216">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="e4ea1-217">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e4ea1-217">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e4ea1-218">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-218">Int32</span></span>|<span data-ttu-id="e4ea1-219">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-219">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e4ea1-220">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e4ea1-220">passwordExpirationDays</span></span>|<span data-ttu-id="e4ea1-221">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-221">Int32</span></span>|<span data-ttu-id="e4ea1-222">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-222">Number of days before the password expires.</span></span> <span data-ttu-id="e4ea1-223">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e4ea1-224">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="e4ea1-224">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="e4ea1-225">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ea1-225">Int32</span></span>|<span data-ttu-id="e4ea1-226">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-226">Number of previous passwords to block.</span></span> <span data-ttu-id="e4ea1-227">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-227">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e4ea1-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e4ea1-228">storageRequireEncryption</span></span>|<span data-ttu-id="e4ea1-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4ea1-229">Boolean</span></span>|<span data-ttu-id="e4ea1-230">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-230">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e4ea1-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4ea1-231">Response</span></span>
<span data-ttu-id="e4ea1-232">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-232">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4ea1-233">Пример</span><span class="sxs-lookup"><span data-stu-id="e4ea1-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4ea1-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4ea1-234">Request</span></span>
<span data-ttu-id="e4ea1-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1160

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

### <a name="response"></a><span data-ttu-id="e4ea1-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4ea1-236">Response</span></span>
<span data-ttu-id="e4ea1-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4ea1-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1332

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




