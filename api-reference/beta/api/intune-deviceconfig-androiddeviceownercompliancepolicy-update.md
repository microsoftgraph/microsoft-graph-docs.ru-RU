---
title: Обновление androidDeviceOwnerCompliancePolicy
description: Обновление свойств объекта AndroidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3dd359839127b16ac9ebb7ae74478a287530694a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133544"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="39d78-103">Обновление androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="39d78-103">Update androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="39d78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39d78-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39d78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39d78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39d78-107">Обновление свойств объекта [AndroidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39d78-107">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39d78-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39d78-108">Prerequisites</span></span>
<span data-ttu-id="39d78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39d78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39d78-111">Permission type</span></span>|<span data-ttu-id="39d78-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39d78-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39d78-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39d78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39d78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39d78-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39d78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39d78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d78-116">Not supported.</span></span>|
|<span data-ttu-id="39d78-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="39d78-117">Application</span></span>|<span data-ttu-id="39d78-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d78-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39d78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39d78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="39d78-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="39d78-120">Request headers</span></span>
|<span data-ttu-id="39d78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39d78-121">Header</span></span>|<span data-ttu-id="39d78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="39d78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39d78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39d78-123">Authorization</span></span>|<span data-ttu-id="39d78-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39d78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39d78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39d78-125">Accept</span></span>|<span data-ttu-id="39d78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39d78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39d78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39d78-127">Request body</span></span>
<span data-ttu-id="39d78-128">В теле запроса поставляем представление JSON для [объекта AndroidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39d78-128">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="39d78-129">В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39d78-129">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="39d78-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="39d78-130">Property</span></span>|<span data-ttu-id="39d78-131">Тип</span><span class="sxs-lookup"><span data-stu-id="39d78-131">Type</span></span>|<span data-ttu-id="39d78-132">Описание</span><span class="sxs-lookup"><span data-stu-id="39d78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d78-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39d78-133">roleScopeTagIds</span></span>|<span data-ttu-id="39d78-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39d78-134">String collection</span></span>|<span data-ttu-id="39d78-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="39d78-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39d78-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-137">id</span><span class="sxs-lookup"><span data-stu-id="39d78-137">id</span></span>|<span data-ttu-id="39d78-138">Строка</span><span class="sxs-lookup"><span data-stu-id="39d78-138">String</span></span>|<span data-ttu-id="39d78-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39d78-139">Key of the entity.</span></span> <span data-ttu-id="39d78-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39d78-141">createdDateTime</span></span>|<span data-ttu-id="39d78-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d78-142">DateTimeOffset</span></span>|<span data-ttu-id="39d78-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="39d78-143">DateTime the object was created.</span></span> <span data-ttu-id="39d78-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-145">description</span><span class="sxs-lookup"><span data-stu-id="39d78-145">description</span></span>|<span data-ttu-id="39d78-146">Строка</span><span class="sxs-lookup"><span data-stu-id="39d78-146">String</span></span>|<span data-ttu-id="39d78-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39d78-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39d78-149">lastModifiedDateTime</span></span>|<span data-ttu-id="39d78-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d78-150">DateTimeOffset</span></span>|<span data-ttu-id="39d78-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="39d78-151">DateTime the object was last modified.</span></span> <span data-ttu-id="39d78-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-153">displayName</span><span class="sxs-lookup"><span data-stu-id="39d78-153">displayName</span></span>|<span data-ttu-id="39d78-154">Строка</span><span class="sxs-lookup"><span data-stu-id="39d78-154">String</span></span>|<span data-ttu-id="39d78-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39d78-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-157">version</span><span class="sxs-lookup"><span data-stu-id="39d78-157">version</span></span>|<span data-ttu-id="39d78-158">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-158">Int32</span></span>|<span data-ttu-id="39d78-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-159">Version of the device configuration.</span></span> <span data-ttu-id="39d78-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39d78-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39d78-161">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="39d78-161">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="39d78-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d78-162">Boolean</span></span>|<span data-ttu-id="39d78-163">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="39d78-163">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="39d78-164">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="39d78-164">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="39d78-165">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="39d78-165">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="39d78-166">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="39d78-166">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="39d78-167">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="39d78-167">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="39d78-168">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="39d78-168">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="39d78-169">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="39d78-169">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="39d78-170">MDATP требует минимального уровня риска для защиты от мобильных угроз, чтобы сообщить о несоблюдении.</span><span class="sxs-lookup"><span data-stu-id="39d78-170">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="39d78-171">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="39d78-171">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="39d78-172">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="39d78-172">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="39d78-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d78-173">Boolean</span></span>|<span data-ttu-id="39d78-174">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="39d78-174">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="39d78-175">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="39d78-175">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="39d78-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d78-176">Boolean</span></span>|<span data-ttu-id="39d78-177">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="39d78-177">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="39d78-178">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="39d78-178">osMinimumVersion</span></span>|<span data-ttu-id="39d78-179">String</span><span class="sxs-lookup"><span data-stu-id="39d78-179">String</span></span>|<span data-ttu-id="39d78-180">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="39d78-180">Minimum Android version.</span></span>|
|<span data-ttu-id="39d78-181">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="39d78-181">osMaximumVersion</span></span>|<span data-ttu-id="39d78-182">String</span><span class="sxs-lookup"><span data-stu-id="39d78-182">String</span></span>|<span data-ttu-id="39d78-183">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="39d78-183">Maximum Android version.</span></span>|
|<span data-ttu-id="39d78-184">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="39d78-184">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="39d78-185">String</span><span class="sxs-lookup"><span data-stu-id="39d78-185">String</span></span>|<span data-ttu-id="39d78-186">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="39d78-186">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="39d78-187">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="39d78-187">passwordRequired</span></span>|<span data-ttu-id="39d78-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d78-188">Boolean</span></span>|<span data-ttu-id="39d78-189">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="39d78-189">Require a password to unlock device.</span></span>|
|<span data-ttu-id="39d78-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="39d78-190">passwordMinimumLength</span></span>|<span data-ttu-id="39d78-191">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-191">Int32</span></span>|<span data-ttu-id="39d78-192">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="39d78-192">Minimum password length.</span></span> <span data-ttu-id="39d78-193">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="39d78-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="39d78-194">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="39d78-194">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="39d78-195">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-195">Int32</span></span>|<span data-ttu-id="39d78-196">Указывает минимальное количество букв, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-196">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="39d78-197">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="39d78-197">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39d78-198">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="39d78-198">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="39d78-199">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-199">Int32</span></span>|<span data-ttu-id="39d78-200">Указывает минимальное число символов более низкого уровня, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-200">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="39d78-201">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="39d78-201">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39d78-202">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="39d78-202">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="39d78-203">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-203">Int32</span></span>|<span data-ttu-id="39d78-204">Указывает минимальное количество символов без букв, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-204">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="39d78-205">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="39d78-205">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39d78-206">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="39d78-206">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="39d78-207">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-207">Int32</span></span>|<span data-ttu-id="39d78-208">Указывает минимальное число числимые символы, необходимые для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-208">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="39d78-209">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="39d78-209">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39d78-210">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="39d78-210">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="39d78-211">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-211">Int32</span></span>|<span data-ttu-id="39d78-212">Указывает минимальное количество символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-212">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="39d78-213">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="39d78-213">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39d78-214">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="39d78-214">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="39d78-215">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-215">Int32</span></span>|<span data-ttu-id="39d78-216">Указывает минимальное количество символов верхней буквы, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="39d78-216">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="39d78-217">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="39d78-217">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39d78-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="39d78-218">passwordRequiredType</span></span>|[<span data-ttu-id="39d78-219">AndroidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="39d78-219">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="39d78-220">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="39d78-220">Type of characters in password.</span></span> <span data-ttu-id="39d78-221">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="39d78-221">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="39d78-222">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="39d78-222">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="39d78-223">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-223">Int32</span></span>|<span data-ttu-id="39d78-224">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="39d78-224">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="39d78-225">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="39d78-225">passwordExpirationDays</span></span>|<span data-ttu-id="39d78-226">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-226">Int32</span></span>|<span data-ttu-id="39d78-227">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="39d78-227">Number of days before the password expires.</span></span> <span data-ttu-id="39d78-228">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="39d78-228">Valid values 1 to 365</span></span>|
|<span data-ttu-id="39d78-229">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="39d78-229">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="39d78-230">Int32</span><span class="sxs-lookup"><span data-stu-id="39d78-230">Int32</span></span>|<span data-ttu-id="39d78-231">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="39d78-231">Number of previous passwords to block.</span></span> <span data-ttu-id="39d78-232">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="39d78-232">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39d78-233">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="39d78-233">storageRequireEncryption</span></span>|<span data-ttu-id="39d78-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d78-234">Boolean</span></span>|<span data-ttu-id="39d78-235">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="39d78-235">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="39d78-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="39d78-236">Response</span></span>
<span data-ttu-id="39d78-237">В случае успешного использования этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="39d78-237">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39d78-238">Пример</span><span class="sxs-lookup"><span data-stu-id="39d78-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="39d78-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="39d78-239">Request</span></span>
<span data-ttu-id="39d78-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39d78-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39d78-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="39d78-241">Response</span></span>
<span data-ttu-id="39d78-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39d78-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




