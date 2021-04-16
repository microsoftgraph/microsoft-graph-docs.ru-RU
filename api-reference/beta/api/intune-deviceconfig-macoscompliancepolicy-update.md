---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4eae08b154553b78b987ca65dc22a8e8fff12eb8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864062"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="e5cf0-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e5cf0-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="e5cf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5cf0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5cf0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5cf0-107">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5cf0-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5cf0-108">Prerequisites</span></span>
<span data-ttu-id="e5cf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5cf0-111">Permission type</span></span>|<span data-ttu-id="e5cf0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5cf0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5cf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5cf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5cf0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cf0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5cf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5cf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5cf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-116">Not supported.</span></span>|
|<span data-ttu-id="e5cf0-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e5cf0-117">Application</span></span>|<span data-ttu-id="e5cf0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cf0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5cf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5cf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e5cf0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5cf0-120">Request headers</span></span>
|<span data-ttu-id="e5cf0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5cf0-121">Header</span></span>|<span data-ttu-id="e5cf0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5cf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5cf0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5cf0-123">Authorization</span></span>|<span data-ttu-id="e5cf0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5cf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5cf0-125">Accept</span></span>|<span data-ttu-id="e5cf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5cf0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5cf0-127">Request body</span></span>
<span data-ttu-id="e5cf0-128">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="e5cf0-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="e5cf0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5cf0-130">Property</span></span>|<span data-ttu-id="e5cf0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5cf0-131">Type</span></span>|<span data-ttu-id="e5cf0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5cf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5cf0-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5cf0-133">roleScopeTagIds</span></span>|<span data-ttu-id="e5cf0-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-134">String collection</span></span>|<span data-ttu-id="e5cf0-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5cf0-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-137">id</span><span class="sxs-lookup"><span data-stu-id="e5cf0-137">id</span></span>|<span data-ttu-id="e5cf0-138">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-138">String</span></span>|<span data-ttu-id="e5cf0-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-139">Key of the entity.</span></span> <span data-ttu-id="e5cf0-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5cf0-141">createdDateTime</span></span>|<span data-ttu-id="e5cf0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5cf0-142">DateTimeOffset</span></span>|<span data-ttu-id="e5cf0-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-143">DateTime the object was created.</span></span> <span data-ttu-id="e5cf0-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-145">description</span><span class="sxs-lookup"><span data-stu-id="e5cf0-145">description</span></span>|<span data-ttu-id="e5cf0-146">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-146">String</span></span>|<span data-ttu-id="e5cf0-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5cf0-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5cf0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e5cf0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5cf0-150">DateTimeOffset</span></span>|<span data-ttu-id="e5cf0-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e5cf0-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e5cf0-153">displayName</span></span>|<span data-ttu-id="e5cf0-154">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-154">String</span></span>|<span data-ttu-id="e5cf0-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5cf0-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-157">version</span><span class="sxs-lookup"><span data-stu-id="e5cf0-157">version</span></span>|<span data-ttu-id="e5cf0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cf0-158">Int32</span></span>|<span data-ttu-id="e5cf0-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-159">Version of the device configuration.</span></span> <span data-ttu-id="e5cf0-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf0-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5cf0-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e5cf0-161">passwordRequired</span></span>|<span data-ttu-id="e5cf0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cf0-162">Boolean</span></span>|<span data-ttu-id="e5cf0-163">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e5cf0-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e5cf0-164">passwordBlockSimple</span></span>|<span data-ttu-id="e5cf0-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cf0-165">Boolean</span></span>|<span data-ttu-id="e5cf0-166">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="e5cf0-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e5cf0-167">passwordExpirationDays</span></span>|<span data-ttu-id="e5cf0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cf0-168">Int32</span></span>|<span data-ttu-id="e5cf0-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-169">Number of days before the password expires.</span></span> <span data-ttu-id="e5cf0-170">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e5cf0-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e5cf0-171">passwordMinimumLength</span></span>|<span data-ttu-id="e5cf0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cf0-172">Int32</span></span>|<span data-ttu-id="e5cf0-173">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-173">Minimum length of password.</span></span> <span data-ttu-id="e5cf0-174">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e5cf0-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e5cf0-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e5cf0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cf0-176">Int32</span></span>|<span data-ttu-id="e5cf0-177">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e5cf0-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e5cf0-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e5cf0-179">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cf0-179">Int32</span></span>|<span data-ttu-id="e5cf0-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-180">Number of previous passwords to block.</span></span> <span data-ttu-id="e5cf0-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e5cf0-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e5cf0-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e5cf0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="e5cf0-183">Int32</span></span>|<span data-ttu-id="e5cf0-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e5cf0-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e5cf0-185">passwordRequiredType</span></span>|[<span data-ttu-id="e5cf0-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e5cf0-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e5cf0-187">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-187">The required password type.</span></span> <span data-ttu-id="e5cf0-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e5cf0-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e5cf0-189">osMinimumVersion</span></span>|<span data-ttu-id="e5cf0-190">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-190">String</span></span>|<span data-ttu-id="e5cf0-191">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="e5cf0-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e5cf0-192">osMaximumVersion</span></span>|<span data-ttu-id="e5cf0-193">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-193">String</span></span>|<span data-ttu-id="e5cf0-194">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="e5cf0-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="e5cf0-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="e5cf0-196">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-196">String</span></span>|<span data-ttu-id="e5cf0-197">Минимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="e5cf0-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="e5cf0-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="e5cf0-199">String</span><span class="sxs-lookup"><span data-stu-id="e5cf0-199">String</span></span>|<span data-ttu-id="e5cf0-200">Максимальная версия сборки MacOS.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="e5cf0-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e5cf0-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="e5cf0-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cf0-202">Boolean</span></span>|<span data-ttu-id="e5cf0-203">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="e5cf0-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e5cf0-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e5cf0-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cf0-205">Boolean</span></span>|<span data-ttu-id="e5cf0-206">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="e5cf0-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e5cf0-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e5cf0-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e5cf0-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e5cf0-209">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e5cf0-210">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e5cf0-211">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e5cf0-211">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e5cf0-212">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e5cf0-212">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e5cf0-213">MDATP требует минимального уровня риска для защиты от мобильных угроз, чтобы сообщить о несоблюдении.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-213">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e5cf0-214">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-214">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e5cf0-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e5cf0-215">storageRequireEncryption</span></span>|<span data-ttu-id="e5cf0-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5cf0-216">Boolean</span></span>|<span data-ttu-id="e5cf0-217">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-217">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="e5cf0-218">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="e5cf0-218">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="e5cf0-219">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="e5cf0-219">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="e5cf0-220">Параметр System и Privacy, который определяет, какие приложения для скачивания можно запускать на macOS-устройстве.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-220">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="e5cf0-221">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-221">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="e5cf0-222">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="e5cf0-222">firewallEnabled</span></span>|<span data-ttu-id="e5cf0-223">Логический</span><span class="sxs-lookup"><span data-stu-id="e5cf0-223">Boolean</span></span>|<span data-ttu-id="e5cf0-224">Следует ли включить брандмауэр или нет.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-224">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="e5cf0-225">брандмауэрBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="e5cf0-225">firewallBlockAllIncoming</span></span>|<span data-ttu-id="e5cf0-226">Логический</span><span class="sxs-lookup"><span data-stu-id="e5cf0-226">Boolean</span></span>|<span data-ttu-id="e5cf0-227">Соответствует параметру "Блокировка всех входящих подключений".</span><span class="sxs-lookup"><span data-stu-id="e5cf0-227">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="e5cf0-228">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="e5cf0-228">firewallEnableStealthMode</span></span>|<span data-ttu-id="e5cf0-229">Логический</span><span class="sxs-lookup"><span data-stu-id="e5cf0-229">Boolean</span></span>|<span data-ttu-id="e5cf0-230">Соответствует режиму "Включить режим стелс".</span><span class="sxs-lookup"><span data-stu-id="e5cf0-230">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="e5cf0-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5cf0-231">Response</span></span>
<span data-ttu-id="e5cf0-232">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-232">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5cf0-233">Пример</span><span class="sxs-lookup"><span data-stu-id="e5cf0-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5cf0-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5cf0-234">Request</span></span>
<span data-ttu-id="e5cf0-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1146

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="e5cf0-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cf0-236">Response</span></span>
<span data-ttu-id="e5cf0-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5cf0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```




