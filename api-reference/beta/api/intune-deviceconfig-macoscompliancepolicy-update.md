---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2eb1e7835d0febcd608f8019557d6955065fab1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797398"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="5b81e-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5b81e-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="5b81e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b81e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b81e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b81e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b81e-106">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b81e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5b81e-107">Prerequisites</span></span>
<span data-ttu-id="5b81e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b81e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b81e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b81e-110">Permission type</span></span>|<span data-ttu-id="5b81e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b81e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b81e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b81e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b81e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b81e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b81e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b81e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b81e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b81e-115">Not supported.</span></span>|
|<span data-ttu-id="5b81e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b81e-116">Application</span></span>|<span data-ttu-id="5b81e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b81e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b81e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b81e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5b81e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b81e-119">Request headers</span></span>
|<span data-ttu-id="5b81e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b81e-120">Header</span></span>|<span data-ttu-id="5b81e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b81e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b81e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b81e-122">Authorization</span></span>|<span data-ttu-id="5b81e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b81e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b81e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b81e-124">Accept</span></span>|<span data-ttu-id="5b81e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b81e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b81e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b81e-126">Request body</span></span>
<span data-ttu-id="5b81e-127">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b81e-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="5b81e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="5b81e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b81e-129">Property</span></span>|<span data-ttu-id="5b81e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5b81e-130">Type</span></span>|<span data-ttu-id="5b81e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5b81e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b81e-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b81e-132">roleScopeTagIds</span></span>|<span data-ttu-id="5b81e-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5b81e-133">String collection</span></span>|<span data-ttu-id="5b81e-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5b81e-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b81e-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-136">id</span><span class="sxs-lookup"><span data-stu-id="5b81e-136">id</span></span>|<span data-ttu-id="5b81e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5b81e-137">String</span></span>|<span data-ttu-id="5b81e-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b81e-138">Key of the entity.</span></span> <span data-ttu-id="5b81e-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b81e-140">createdDateTime</span></span>|<span data-ttu-id="5b81e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b81e-141">DateTimeOffset</span></span>|<span data-ttu-id="5b81e-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5b81e-142">DateTime the object was created.</span></span> <span data-ttu-id="5b81e-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-144">description</span><span class="sxs-lookup"><span data-stu-id="5b81e-144">description</span></span>|<span data-ttu-id="5b81e-145">String</span><span class="sxs-lookup"><span data-stu-id="5b81e-145">String</span></span>|<span data-ttu-id="5b81e-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b81e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b81e-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b81e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="5b81e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b81e-149">DateTimeOffset</span></span>|<span data-ttu-id="5b81e-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5b81e-150">DateTime the object was last modified.</span></span> <span data-ttu-id="5b81e-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="5b81e-152">displayName</span></span>|<span data-ttu-id="5b81e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="5b81e-153">String</span></span>|<span data-ttu-id="5b81e-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b81e-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b81e-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-156">version</span><span class="sxs-lookup"><span data-stu-id="5b81e-156">version</span></span>|<span data-ttu-id="5b81e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5b81e-157">Int32</span></span>|<span data-ttu-id="5b81e-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b81e-158">Version of the device configuration.</span></span> <span data-ttu-id="5b81e-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b81e-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b81e-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5b81e-160">passwordRequired</span></span>|<span data-ttu-id="5b81e-161">Логический</span><span class="sxs-lookup"><span data-stu-id="5b81e-161">Boolean</span></span>|<span data-ttu-id="5b81e-162">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5b81e-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="5b81e-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5b81e-163">passwordBlockSimple</span></span>|<span data-ttu-id="5b81e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-164">Boolean</span></span>|<span data-ttu-id="5b81e-165">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="5b81e-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="5b81e-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5b81e-166">passwordExpirationDays</span></span>|<span data-ttu-id="5b81e-167">Int32</span><span class="sxs-lookup"><span data-stu-id="5b81e-167">Int32</span></span>|<span data-ttu-id="5b81e-168">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="5b81e-168">Number of days before the password expires.</span></span> <span data-ttu-id="5b81e-169">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="5b81e-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="5b81e-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5b81e-170">passwordMinimumLength</span></span>|<span data-ttu-id="5b81e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5b81e-171">Int32</span></span>|<span data-ttu-id="5b81e-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5b81e-172">Minimum length of password.</span></span> <span data-ttu-id="5b81e-173">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="5b81e-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="5b81e-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5b81e-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5b81e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="5b81e-175">Int32</span></span>|<span data-ttu-id="5b81e-176">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5b81e-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5b81e-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5b81e-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5b81e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="5b81e-178">Int32</span></span>|<span data-ttu-id="5b81e-179">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="5b81e-179">Number of previous passwords to block.</span></span> <span data-ttu-id="5b81e-180">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="5b81e-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5b81e-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5b81e-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5b81e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="5b81e-182">Int32</span></span>|<span data-ttu-id="5b81e-183">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5b81e-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5b81e-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5b81e-184">passwordRequiredType</span></span>|[<span data-ttu-id="5b81e-185">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="5b81e-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5b81e-186">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="5b81e-186">The required password type.</span></span> <span data-ttu-id="5b81e-187">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5b81e-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5b81e-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5b81e-188">osMinimumVersion</span></span>|<span data-ttu-id="5b81e-189">String</span><span class="sxs-lookup"><span data-stu-id="5b81e-189">String</span></span>|<span data-ttu-id="5b81e-190">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="5b81e-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="5b81e-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5b81e-191">osMaximumVersion</span></span>|<span data-ttu-id="5b81e-192">String</span><span class="sxs-lookup"><span data-stu-id="5b81e-192">String</span></span>|<span data-ttu-id="5b81e-193">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="5b81e-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="5b81e-194">Осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="5b81e-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="5b81e-195">String</span><span class="sxs-lookup"><span data-stu-id="5b81e-195">String</span></span>|<span data-ttu-id="5b81e-196">Минимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="5b81e-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="5b81e-197">Осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="5b81e-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="5b81e-198">String</span><span class="sxs-lookup"><span data-stu-id="5b81e-198">String</span></span>|<span data-ttu-id="5b81e-199">Максимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="5b81e-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="5b81e-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5b81e-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="5b81e-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-201">Boolean</span></span>|<span data-ttu-id="5b81e-202">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="5b81e-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="5b81e-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5b81e-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5b81e-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-204">Boolean</span></span>|<span data-ttu-id="5b81e-205">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="5b81e-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5b81e-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5b81e-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5b81e-207">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="5b81e-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5b81e-208">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="5b81e-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5b81e-209">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5b81e-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5b81e-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5b81e-210">storageRequireEncryption</span></span>|<span data-ttu-id="5b81e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-211">Boolean</span></span>|<span data-ttu-id="5b81e-212">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="5b81e-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="5b81e-213">Гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="5b81e-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="5b81e-214">Макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="5b81e-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="5b81e-215">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="5b81e-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="5b81e-216">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="5b81e-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="5b81e-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="5b81e-217">firewallEnabled</span></span>|<span data-ttu-id="5b81e-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-218">Boolean</span></span>|<span data-ttu-id="5b81e-219">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="5b81e-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="5b81e-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="5b81e-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="5b81e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-221">Boolean</span></span>|<span data-ttu-id="5b81e-222">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="5b81e-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="5b81e-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="5b81e-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="5b81e-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b81e-224">Boolean</span></span>|<span data-ttu-id="5b81e-225">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="5b81e-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="5b81e-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b81e-226">Response</span></span>
<span data-ttu-id="5b81e-227">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b81e-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b81e-228">Пример</span><span class="sxs-lookup"><span data-stu-id="5b81e-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b81e-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b81e-229">Request</span></span>
<span data-ttu-id="5b81e-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b81e-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b81e-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b81e-231">Response</span></span>
<span data-ttu-id="5b81e-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b81e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





