---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25e06ae2e7a467c4bc61506bb9b6694b5c3b9bbe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086104"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="f4cb7-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f4cb7-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="f4cb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4cb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4cb7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4cb7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4cb7-107">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-107">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4cb7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f4cb7-108">Prerequisites</span></span>
<span data-ttu-id="f4cb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4cb7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4cb7-111">Permission type</span></span>|<span data-ttu-id="f4cb7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4cb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4cb7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4cb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4cb7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cb7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4cb7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4cb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4cb7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-116">Not supported.</span></span>|
|<span data-ttu-id="f4cb7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4cb7-117">Application</span></span>|<span data-ttu-id="f4cb7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cb7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4cb7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4cb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f4cb7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4cb7-120">Request headers</span></span>
|<span data-ttu-id="f4cb7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4cb7-121">Header</span></span>|<span data-ttu-id="f4cb7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4cb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4cb7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4cb7-123">Authorization</span></span>|<span data-ttu-id="f4cb7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4cb7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4cb7-125">Accept</span></span>|<span data-ttu-id="f4cb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4cb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4cb7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4cb7-127">Request body</span></span>
<span data-ttu-id="f4cb7-128">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-128">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="f4cb7-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-129">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="f4cb7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4cb7-130">Property</span></span>|<span data-ttu-id="f4cb7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f4cb7-131">Type</span></span>|<span data-ttu-id="f4cb7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f4cb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4cb7-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4cb7-133">roleScopeTagIds</span></span>|<span data-ttu-id="f4cb7-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f4cb7-134">String collection</span></span>|<span data-ttu-id="f4cb7-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4cb7-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-137">id</span><span class="sxs-lookup"><span data-stu-id="f4cb7-137">id</span></span>|<span data-ttu-id="f4cb7-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f4cb7-138">String</span></span>|<span data-ttu-id="f4cb7-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-139">Key of the entity.</span></span> <span data-ttu-id="f4cb7-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4cb7-141">createdDateTime</span></span>|<span data-ttu-id="f4cb7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4cb7-142">DateTimeOffset</span></span>|<span data-ttu-id="f4cb7-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-143">DateTime the object was created.</span></span> <span data-ttu-id="f4cb7-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-145">description</span><span class="sxs-lookup"><span data-stu-id="f4cb7-145">description</span></span>|<span data-ttu-id="f4cb7-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f4cb7-146">String</span></span>|<span data-ttu-id="f4cb7-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4cb7-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4cb7-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f4cb7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4cb7-150">DateTimeOffset</span></span>|<span data-ttu-id="f4cb7-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-151">DateTime the object was last modified.</span></span> <span data-ttu-id="f4cb7-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-153">displayName</span><span class="sxs-lookup"><span data-stu-id="f4cb7-153">displayName</span></span>|<span data-ttu-id="f4cb7-154">Строка</span><span class="sxs-lookup"><span data-stu-id="f4cb7-154">String</span></span>|<span data-ttu-id="f4cb7-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4cb7-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-157">version</span><span class="sxs-lookup"><span data-stu-id="f4cb7-157">version</span></span>|<span data-ttu-id="f4cb7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cb7-158">Int32</span></span>|<span data-ttu-id="f4cb7-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-159">Version of the device configuration.</span></span> <span data-ttu-id="f4cb7-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4cb7-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f4cb7-161">passwordRequired</span></span>|<span data-ttu-id="f4cb7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-162">Boolean</span></span>|<span data-ttu-id="f4cb7-163">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="f4cb7-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f4cb7-164">passwordBlockSimple</span></span>|<span data-ttu-id="f4cb7-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-165">Boolean</span></span>|<span data-ttu-id="f4cb7-166">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f4cb7-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f4cb7-167">passwordMinimumLength</span></span>|<span data-ttu-id="f4cb7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cb7-168">Int32</span></span>|<span data-ttu-id="f4cb7-169">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-169">Minimum password length.</span></span> <span data-ttu-id="f4cb7-170">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f4cb7-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f4cb7-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f4cb7-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cb7-172">Int32</span></span>|<span data-ttu-id="f4cb7-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f4cb7-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f4cb7-174">passwordRequiredType</span></span>|[<span data-ttu-id="f4cb7-175">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f4cb7-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f4cb7-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-176">The required password type.</span></span> <span data-ttu-id="f4cb7-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f4cb7-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f4cb7-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f4cb7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cb7-179">Int32</span></span>|<span data-ttu-id="f4cb7-180">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="f4cb7-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f4cb7-181">passwordExpirationDays</span></span>|<span data-ttu-id="f4cb7-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cb7-182">Int32</span></span>|<span data-ttu-id="f4cb7-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-183">Number of days before password expiration.</span></span> <span data-ttu-id="f4cb7-184">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="f4cb7-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f4cb7-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f4cb7-186">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cb7-186">Int32</span></span>|<span data-ttu-id="f4cb7-187">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f4cb7-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="f4cb7-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="f4cb7-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-189">Boolean</span></span>|<span data-ttu-id="f4cb7-190">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="f4cb7-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f4cb7-191">osMinimumVersion</span></span>|<span data-ttu-id="f4cb7-192">String</span><span class="sxs-lookup"><span data-stu-id="f4cb7-192">String</span></span>|<span data-ttu-id="f4cb7-193">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f4cb7-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f4cb7-194">osMaximumVersion</span></span>|<span data-ttu-id="f4cb7-195">String</span><span class="sxs-lookup"><span data-stu-id="f4cb7-195">String</span></span>|<span data-ttu-id="f4cb7-196">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f4cb7-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="f4cb7-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="f4cb7-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-198">Boolean</span></span>|<span data-ttu-id="f4cb7-199">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="f4cb7-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="f4cb7-200">bitLockerEnabled</span></span>|<span data-ttu-id="f4cb7-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-201">Boolean</span></span>|<span data-ttu-id="f4cb7-202">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="f4cb7-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="f4cb7-203">secureBootEnabled</span></span>|<span data-ttu-id="f4cb7-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-204">Boolean</span></span>|<span data-ttu-id="f4cb7-205">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="f4cb7-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="f4cb7-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="f4cb7-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="f4cb7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-207">Boolean</span></span>|<span data-ttu-id="f4cb7-208">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f4cb7-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f4cb7-209">storageRequireEncryption</span></span>|<span data-ttu-id="f4cb7-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-210">Boolean</span></span>|<span data-ttu-id="f4cb7-211">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="f4cb7-212">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="f4cb7-212">activeFirewallRequired</span></span>|<span data-ttu-id="f4cb7-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4cb7-213">Boolean</span></span>|<span data-ttu-id="f4cb7-214">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="f4cb7-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="f4cb7-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="f4cb7-216">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="f4cb7-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="f4cb7-217">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="f4cb7-218">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f4cb7-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4cb7-219">Response</span></span>
<span data-ttu-id="f4cb7-220">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-220">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4cb7-221">Пример</span><span class="sxs-lookup"><span data-stu-id="f4cb7-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4cb7-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4cb7-222">Request</span></span>
<span data-ttu-id="f4cb7-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f4cb7-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4cb7-224">Response</span></span>
<span data-ttu-id="f4cb7-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4cb7-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```






