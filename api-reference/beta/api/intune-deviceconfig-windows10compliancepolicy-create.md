---
title: Создание windows10CompliancePolicy
description: Создает объект windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e69151a5f0b7a0bc8c0558fc9f178714e7520d1c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792641"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="5eaa1-103">Создание windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5eaa1-103">Create windows10CompliancePolicy</span></span>

<span data-ttu-id="5eaa1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eaa1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5eaa1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5eaa1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eaa1-107">Создает объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5eaa1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5eaa1-108">Prerequisites</span></span>
<span data-ttu-id="5eaa1-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5eaa1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eaa1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eaa1-111">Permission type</span></span>|<span data-ttu-id="5eaa1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eaa1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eaa1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eaa1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5eaa1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eaa1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5eaa1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eaa1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eaa1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-116">Not supported.</span></span>|
|<span data-ttu-id="5eaa1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eaa1-117">Application</span></span>|<span data-ttu-id="5eaa1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eaa1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eaa1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eaa1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5eaa1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5eaa1-120">Request headers</span></span>
|<span data-ttu-id="5eaa1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5eaa1-121">Header</span></span>|<span data-ttu-id="5eaa1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5eaa1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eaa1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5eaa1-123">Authorization</span></span>|<span data-ttu-id="5eaa1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eaa1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5eaa1-125">Accept</span></span>|<span data-ttu-id="5eaa1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5eaa1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eaa1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5eaa1-127">Request body</span></span>
<span data-ttu-id="5eaa1-128">В теле запроса добавьте представление объекта windows10CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="5eaa1-129">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="5eaa1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5eaa1-130">Property</span></span>|<span data-ttu-id="5eaa1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5eaa1-131">Type</span></span>|<span data-ttu-id="5eaa1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5eaa1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eaa1-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5eaa1-133">roleScopeTagIds</span></span>|<span data-ttu-id="5eaa1-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-134">String collection</span></span>|<span data-ttu-id="5eaa1-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5eaa1-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-137">id</span><span class="sxs-lookup"><span data-stu-id="5eaa1-137">id</span></span>|<span data-ttu-id="5eaa1-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5eaa1-138">String</span></span>|<span data-ttu-id="5eaa1-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-139">Key of the entity.</span></span> <span data-ttu-id="5eaa1-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5eaa1-141">createdDateTime</span></span>|<span data-ttu-id="5eaa1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eaa1-142">DateTimeOffset</span></span>|<span data-ttu-id="5eaa1-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-143">DateTime the object was created.</span></span> <span data-ttu-id="5eaa1-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-145">description</span><span class="sxs-lookup"><span data-stu-id="5eaa1-145">description</span></span>|<span data-ttu-id="5eaa1-146">String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-146">String</span></span>|<span data-ttu-id="5eaa1-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5eaa1-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eaa1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="5eaa1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eaa1-150">DateTimeOffset</span></span>|<span data-ttu-id="5eaa1-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-151">DateTime the object was last modified.</span></span> <span data-ttu-id="5eaa1-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-153">displayName</span><span class="sxs-lookup"><span data-stu-id="5eaa1-153">displayName</span></span>|<span data-ttu-id="5eaa1-154">Строка</span><span class="sxs-lookup"><span data-stu-id="5eaa1-154">String</span></span>|<span data-ttu-id="5eaa1-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5eaa1-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-157">version</span><span class="sxs-lookup"><span data-stu-id="5eaa1-157">version</span></span>|<span data-ttu-id="5eaa1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5eaa1-158">Int32</span></span>|<span data-ttu-id="5eaa1-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-159">Version of the device configuration.</span></span> <span data-ttu-id="5eaa1-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5eaa1-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5eaa1-161">passwordRequired</span></span>|<span data-ttu-id="5eaa1-162">Логический</span><span class="sxs-lookup"><span data-stu-id="5eaa1-162">Boolean</span></span>|<span data-ttu-id="5eaa1-163">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="5eaa1-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5eaa1-164">passwordBlockSimple</span></span>|<span data-ttu-id="5eaa1-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-165">Boolean</span></span>|<span data-ttu-id="5eaa1-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="5eaa1-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="5eaa1-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="5eaa1-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-168">Boolean</span></span>|<span data-ttu-id="5eaa1-169">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="5eaa1-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5eaa1-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5eaa1-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5eaa1-171">Int32</span></span>|<span data-ttu-id="5eaa1-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5eaa1-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5eaa1-173">passwordExpirationDays</span></span>|<span data-ttu-id="5eaa1-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5eaa1-174">Int32</span></span>|<span data-ttu-id="5eaa1-175">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-175">The password expiration in days.</span></span>|
|<span data-ttu-id="5eaa1-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5eaa1-176">passwordMinimumLength</span></span>|<span data-ttu-id="5eaa1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5eaa1-177">Int32</span></span>|<span data-ttu-id="5eaa1-178">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-178">The minimum password length.</span></span>|
|<span data-ttu-id="5eaa1-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5eaa1-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5eaa1-180">Int32</span><span class="sxs-lookup"><span data-stu-id="5eaa1-180">Int32</span></span>|<span data-ttu-id="5eaa1-181">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5eaa1-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5eaa1-182">passwordRequiredType</span></span>|[<span data-ttu-id="5eaa1-183">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="5eaa1-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5eaa1-184">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-184">The required password type.</span></span> <span data-ttu-id="5eaa1-185">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5eaa1-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5eaa1-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5eaa1-187">Int32</span><span class="sxs-lookup"><span data-stu-id="5eaa1-187">Int32</span></span>|<span data-ttu-id="5eaa1-188">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="5eaa1-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="5eaa1-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="5eaa1-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-190">Boolean</span></span>|<span data-ttu-id="5eaa1-191">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5eaa1-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5eaa1-192">osMinimumVersion</span></span>|<span data-ttu-id="5eaa1-193">String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-193">String</span></span>|<span data-ttu-id="5eaa1-194">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="5eaa1-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5eaa1-195">osMaximumVersion</span></span>|<span data-ttu-id="5eaa1-196">String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-196">String</span></span>|<span data-ttu-id="5eaa1-197">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="5eaa1-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5eaa1-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="5eaa1-199">String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-199">String</span></span>|<span data-ttu-id="5eaa1-200">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="5eaa1-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5eaa1-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="5eaa1-202">String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-202">String</span></span>|<span data-ttu-id="5eaa1-203">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="5eaa1-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="5eaa1-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="5eaa1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-205">Boolean</span></span>|<span data-ttu-id="5eaa1-206">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="5eaa1-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="5eaa1-207">bitLockerEnabled</span></span>|<span data-ttu-id="5eaa1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-208">Boolean</span></span>|<span data-ttu-id="5eaa1-209">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="5eaa1-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="5eaa1-210">secureBootEnabled</span></span>|<span data-ttu-id="5eaa1-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-211">Boolean</span></span>|<span data-ttu-id="5eaa1-212">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="5eaa1-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="5eaa1-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="5eaa1-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-214">Boolean</span></span>|<span data-ttu-id="5eaa1-215">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5eaa1-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5eaa1-216">storageRequireEncryption</span></span>|<span data-ttu-id="5eaa1-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-217">Boolean</span></span>|<span data-ttu-id="5eaa1-218">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="5eaa1-219">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="5eaa1-219">activeFirewallRequired</span></span>|<span data-ttu-id="5eaa1-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-220">Boolean</span></span>|<span data-ttu-id="5eaa1-221">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="5eaa1-222">дефендеренаблед</span><span class="sxs-lookup"><span data-stu-id="5eaa1-222">defenderEnabled</span></span>|<span data-ttu-id="5eaa1-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-223">Boolean</span></span>|<span data-ttu-id="5eaa1-224">Требуется антивредоносная программа защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="5eaa1-225">дефендерверсион</span><span class="sxs-lookup"><span data-stu-id="5eaa1-225">defenderVersion</span></span>|<span data-ttu-id="5eaa1-226">String</span><span class="sxs-lookup"><span data-stu-id="5eaa1-226">String</span></span>|<span data-ttu-id="5eaa1-227">Требовать минимальную версию защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="5eaa1-228">сигнатуреаутофдате</span><span class="sxs-lookup"><span data-stu-id="5eaa1-228">signatureOutOfDate</span></span>|<span data-ttu-id="5eaa1-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-229">Boolean</span></span>|<span data-ttu-id="5eaa1-230">Обязательное обновление подписи антивредоносной программы защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="5eaa1-231">ртпенаблед</span><span class="sxs-lookup"><span data-stu-id="5eaa1-231">rtpEnabled</span></span>|<span data-ttu-id="5eaa1-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-232">Boolean</span></span>|<span data-ttu-id="5eaa1-233">Требование защиты от вредоносных программ Защитника Windows в режиме реального времени на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="5eaa1-234">антивирусрекуиред</span><span class="sxs-lookup"><span data-stu-id="5eaa1-234">antivirusRequired</span></span>|<span data-ttu-id="5eaa1-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-235">Boolean</span></span>|<span data-ttu-id="5eaa1-236">Требование наличия антивирусных решений, зарегистрированных в Windows Декурити Center для включения и отслеживания (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="5eaa1-237">антиспиваререкуиред</span><span class="sxs-lookup"><span data-stu-id="5eaa1-237">antiSpywareRequired</span></span>|<span data-ttu-id="5eaa1-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-238">Boolean</span></span>|<span data-ttu-id="5eaa1-239">Обязательное решение для защиты от шпионских программ, зарегистрированное в Windows Декурити Center для включения и мониторинга (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="5eaa1-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="5eaa1-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="5eaa1-241">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="5eaa1-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="5eaa1-242">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="5eaa1-243">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="5eaa1-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5eaa1-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5eaa1-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-245">Boolean</span></span>|<span data-ttu-id="5eaa1-246">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5eaa1-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5eaa1-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5eaa1-248">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="5eaa1-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5eaa1-249">Потребовать минимального уровня риска для защиты от угроз для отчетов о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5eaa1-250">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5eaa1-251">конфигуратионманажеркомплианцерекуиред</span><span class="sxs-lookup"><span data-stu-id="5eaa1-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="5eaa1-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-252">Boolean</span></span>|<span data-ttu-id="5eaa1-253">Необходимо учитывать состояние соответствия SCCM в отношении состояния соответствия Intune.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="5eaa1-254">тпмрекуиред</span><span class="sxs-lookup"><span data-stu-id="5eaa1-254">tpmRequired</span></span>|<span data-ttu-id="5eaa1-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eaa1-255">Boolean</span></span>|<span data-ttu-id="5eaa1-256">Требуется наличие доверенного платформенного модуля (TPM).</span><span class="sxs-lookup"><span data-stu-id="5eaa1-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="5eaa1-257">девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="5eaa1-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="5eaa1-258">девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="5eaa1-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="5eaa1-259">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5eaa1-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eaa1-260">Response</span></span>
<span data-ttu-id="5eaa1-261">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-261">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eaa1-262">Пример</span><span class="sxs-lookup"><span data-stu-id="5eaa1-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="5eaa1-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eaa1-263">Request</span></span>
<span data-ttu-id="5eaa1-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1911

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="5eaa1-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eaa1-265">Response</span></span>
<span data-ttu-id="5eaa1-266">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-266">Here is an example of the response.</span></span> <span data-ttu-id="5eaa1-267">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-267">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5eaa1-268">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5eaa1-268">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2083

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```



