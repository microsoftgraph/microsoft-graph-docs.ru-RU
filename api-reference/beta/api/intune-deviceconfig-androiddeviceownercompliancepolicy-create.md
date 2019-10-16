---
title: Создание Андроиддевицеовнеркомплианцеполици
description: Создание нового объекта Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59c1ac6078c1b8ebb4477266b1fce43fc18a98a8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534871"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="1acc7-103">Создание Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="1acc7-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="1acc7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1acc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1acc7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1acc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1acc7-106">Создание нового объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1acc7-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1acc7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1acc7-107">Prerequisites</span></span>
<span data-ttu-id="1acc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1acc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1acc7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1acc7-110">Permission type</span></span>|<span data-ttu-id="1acc7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1acc7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1acc7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1acc7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1acc7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1acc7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1acc7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1acc7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1acc7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1acc7-115">Not supported.</span></span>|
|<span data-ttu-id="1acc7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1acc7-116">Application</span></span>|<span data-ttu-id="1acc7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1acc7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1acc7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1acc7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1acc7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1acc7-119">Request headers</span></span>
|<span data-ttu-id="1acc7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1acc7-120">Header</span></span>|<span data-ttu-id="1acc7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1acc7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1acc7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1acc7-122">Authorization</span></span>|<span data-ttu-id="1acc7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1acc7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1acc7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1acc7-124">Accept</span></span>|<span data-ttu-id="1acc7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1acc7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1acc7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1acc7-126">Request body</span></span>
<span data-ttu-id="1acc7-127">В тексте запроса добавьте представление объекта Андроиддевицеовнеркомплианцеполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1acc7-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="1acc7-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеркомплианцеполици.</span><span class="sxs-lookup"><span data-stu-id="1acc7-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="1acc7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1acc7-129">Property</span></span>|<span data-ttu-id="1acc7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1acc7-130">Type</span></span>|<span data-ttu-id="1acc7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1acc7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1acc7-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1acc7-132">roleScopeTagIds</span></span>|<span data-ttu-id="1acc7-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1acc7-133">String collection</span></span>|<span data-ttu-id="1acc7-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1acc7-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1acc7-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-136">id</span><span class="sxs-lookup"><span data-stu-id="1acc7-136">id</span></span>|<span data-ttu-id="1acc7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1acc7-137">String</span></span>|<span data-ttu-id="1acc7-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1acc7-138">Key of the entity.</span></span> <span data-ttu-id="1acc7-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1acc7-140">createdDateTime</span></span>|<span data-ttu-id="1acc7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acc7-141">DateTimeOffset</span></span>|<span data-ttu-id="1acc7-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1acc7-142">DateTime the object was created.</span></span> <span data-ttu-id="1acc7-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-144">description</span><span class="sxs-lookup"><span data-stu-id="1acc7-144">description</span></span>|<span data-ttu-id="1acc7-145">String</span><span class="sxs-lookup"><span data-stu-id="1acc7-145">String</span></span>|<span data-ttu-id="1acc7-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1acc7-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1acc7-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1acc7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acc7-149">DateTimeOffset</span></span>|<span data-ttu-id="1acc7-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1acc7-150">DateTime the object was last modified.</span></span> <span data-ttu-id="1acc7-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-152">displayName</span><span class="sxs-lookup"><span data-stu-id="1acc7-152">displayName</span></span>|<span data-ttu-id="1acc7-153">Строка</span><span class="sxs-lookup"><span data-stu-id="1acc7-153">String</span></span>|<span data-ttu-id="1acc7-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1acc7-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-156">version</span><span class="sxs-lookup"><span data-stu-id="1acc7-156">version</span></span>|<span data-ttu-id="1acc7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-157">Int32</span></span>|<span data-ttu-id="1acc7-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-158">Version of the device configuration.</span></span> <span data-ttu-id="1acc7-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1acc7-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1acc7-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1acc7-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="1acc7-161">Логический</span><span class="sxs-lookup"><span data-stu-id="1acc7-161">Boolean</span></span>|<span data-ttu-id="1acc7-162">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="1acc7-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="1acc7-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="1acc7-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="1acc7-164">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="1acc7-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="1acc7-165">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="1acc7-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1acc7-166">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1acc7-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1acc7-167">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="1acc7-167">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="1acc7-168">Логический</span><span class="sxs-lookup"><span data-stu-id="1acc7-168">Boolean</span></span>|<span data-ttu-id="1acc7-169">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="1acc7-169">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="1acc7-170">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="1acc7-170">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="1acc7-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="1acc7-171">Boolean</span></span>|<span data-ttu-id="1acc7-172">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="1acc7-172">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="1acc7-173">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1acc7-173">osMinimumVersion</span></span>|<span data-ttu-id="1acc7-174">String</span><span class="sxs-lookup"><span data-stu-id="1acc7-174">String</span></span>|<span data-ttu-id="1acc7-175">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="1acc7-175">Minimum Android version.</span></span>|
|<span data-ttu-id="1acc7-176">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1acc7-176">osMaximumVersion</span></span>|<span data-ttu-id="1acc7-177">String</span><span class="sxs-lookup"><span data-stu-id="1acc7-177">String</span></span>|<span data-ttu-id="1acc7-178">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="1acc7-178">Maximum Android version.</span></span>|
|<span data-ttu-id="1acc7-179">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1acc7-179">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="1acc7-180">String</span><span class="sxs-lookup"><span data-stu-id="1acc7-180">String</span></span>|<span data-ttu-id="1acc7-181">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="1acc7-181">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="1acc7-182">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1acc7-182">passwordRequired</span></span>|<span data-ttu-id="1acc7-183">Логический</span><span class="sxs-lookup"><span data-stu-id="1acc7-183">Boolean</span></span>|<span data-ttu-id="1acc7-184">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="1acc7-184">Require a password to unlock device.</span></span>|
|<span data-ttu-id="1acc7-185">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1acc7-185">passwordMinimumLength</span></span>|<span data-ttu-id="1acc7-186">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-186">Int32</span></span>|<span data-ttu-id="1acc7-187">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="1acc7-187">Minimum password length.</span></span> <span data-ttu-id="1acc7-188">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-188">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1acc7-189">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="1acc7-189">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="1acc7-190">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-190">Int32</span></span>|<span data-ttu-id="1acc7-191">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-191">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="1acc7-192">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1acc7-193">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="1acc7-193">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="1acc7-194">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-194">Int32</span></span>|<span data-ttu-id="1acc7-195">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-195">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="1acc7-196">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1acc7-197">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="1acc7-197">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="1acc7-198">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-198">Int32</span></span>|<span data-ttu-id="1acc7-199">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-199">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="1acc7-200">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1acc7-201">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="1acc7-201">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="1acc7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-202">Int32</span></span>|<span data-ttu-id="1acc7-203">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-203">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="1acc7-204">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1acc7-205">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="1acc7-205">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="1acc7-206">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-206">Int32</span></span>|<span data-ttu-id="1acc7-207">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-207">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="1acc7-208">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1acc7-209">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="1acc7-209">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="1acc7-210">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-210">Int32</span></span>|<span data-ttu-id="1acc7-211">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-211">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="1acc7-212">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1acc7-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1acc7-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1acc7-213">passwordRequiredType</span></span>|[<span data-ttu-id="1acc7-214">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1acc7-214">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1acc7-215">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="1acc7-215">Type of characters in password.</span></span> <span data-ttu-id="1acc7-216">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="1acc7-216">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="1acc7-217">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1acc7-217">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1acc7-218">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-218">Int32</span></span>|<span data-ttu-id="1acc7-219">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="1acc7-219">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1acc7-220">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1acc7-220">passwordExpirationDays</span></span>|<span data-ttu-id="1acc7-221">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-221">Int32</span></span>|<span data-ttu-id="1acc7-222">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="1acc7-222">Number of days before the password expires.</span></span> <span data-ttu-id="1acc7-223">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="1acc7-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1acc7-224">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="1acc7-224">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1acc7-225">Int32</span><span class="sxs-lookup"><span data-stu-id="1acc7-225">Int32</span></span>|<span data-ttu-id="1acc7-226">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="1acc7-226">Number of previous passwords to block.</span></span> <span data-ttu-id="1acc7-227">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="1acc7-227">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1acc7-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1acc7-228">storageRequireEncryption</span></span>|<span data-ttu-id="1acc7-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="1acc7-229">Boolean</span></span>|<span data-ttu-id="1acc7-230">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="1acc7-230">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="1acc7-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="1acc7-231">Response</span></span>
<span data-ttu-id="1acc7-232">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1acc7-232">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1acc7-233">Пример</span><span class="sxs-lookup"><span data-stu-id="1acc7-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="1acc7-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="1acc7-234">Request</span></span>
<span data-ttu-id="1acc7-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1acc7-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="1acc7-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="1acc7-236">Response</span></span>
<span data-ttu-id="1acc7-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1acc7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






