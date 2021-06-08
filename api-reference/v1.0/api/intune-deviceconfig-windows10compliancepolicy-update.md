---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b63f2665a081263deae42cd6b66e370a90ee61d9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760568"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="f731a-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f731a-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="f731a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f731a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f731a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f731a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f731a-106">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-106">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f731a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f731a-107">Prerequisites</span></span>
<span data-ttu-id="f731a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f731a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f731a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f731a-110">Permission type</span></span>|<span data-ttu-id="f731a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f731a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f731a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f731a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f731a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f731a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f731a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f731a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f731a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f731a-115">Not supported.</span></span>|
|<span data-ttu-id="f731a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f731a-116">Application</span></span>|<span data-ttu-id="f731a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f731a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f731a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f731a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f731a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f731a-119">Request headers</span></span>
|<span data-ttu-id="f731a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f731a-120">Header</span></span>|<span data-ttu-id="f731a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f731a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f731a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f731a-122">Authorization</span></span>|<span data-ttu-id="f731a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f731a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f731a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f731a-124">Accept</span></span>|<span data-ttu-id="f731a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f731a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f731a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f731a-126">Request body</span></span>
<span data-ttu-id="f731a-127">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f731a-127">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="f731a-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-128">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="f731a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f731a-129">Property</span></span>|<span data-ttu-id="f731a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f731a-130">Type</span></span>|<span data-ttu-id="f731a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f731a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f731a-132">id</span><span class="sxs-lookup"><span data-stu-id="f731a-132">id</span></span>|<span data-ttu-id="f731a-133">String</span><span class="sxs-lookup"><span data-stu-id="f731a-133">String</span></span>|<span data-ttu-id="f731a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f731a-134">Key of the entity.</span></span> <span data-ttu-id="f731a-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f731a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f731a-136">createdDateTime</span></span>|<span data-ttu-id="f731a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f731a-137">DateTimeOffset</span></span>|<span data-ttu-id="f731a-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f731a-138">DateTime the object was created.</span></span> <span data-ttu-id="f731a-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f731a-140">description</span><span class="sxs-lookup"><span data-stu-id="f731a-140">description</span></span>|<span data-ttu-id="f731a-141">String</span><span class="sxs-lookup"><span data-stu-id="f731a-141">String</span></span>|<span data-ttu-id="f731a-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f731a-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f731a-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f731a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f731a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f731a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f731a-145">DateTimeOffset</span></span>|<span data-ttu-id="f731a-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f731a-146">DateTime the object was last modified.</span></span> <span data-ttu-id="f731a-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f731a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f731a-148">displayName</span></span>|<span data-ttu-id="f731a-149">String</span><span class="sxs-lookup"><span data-stu-id="f731a-149">String</span></span>|<span data-ttu-id="f731a-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f731a-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f731a-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f731a-152">version</span><span class="sxs-lookup"><span data-stu-id="f731a-152">version</span></span>|<span data-ttu-id="f731a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f731a-153">Int32</span></span>|<span data-ttu-id="f731a-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f731a-154">Version of the device configuration.</span></span> <span data-ttu-id="f731a-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f731a-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f731a-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f731a-156">passwordRequired</span></span>|<span data-ttu-id="f731a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-157">Boolean</span></span>|<span data-ttu-id="f731a-158">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="f731a-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="f731a-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f731a-159">passwordBlockSimple</span></span>|<span data-ttu-id="f731a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-160">Boolean</span></span>|<span data-ttu-id="f731a-161">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="f731a-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="f731a-162">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="f731a-162">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="f731a-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-163">Boolean</span></span>|<span data-ttu-id="f731a-164">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="f731a-164">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="f731a-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f731a-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f731a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f731a-166">Int32</span></span>|<span data-ttu-id="f731a-167">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f731a-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f731a-168">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f731a-168">passwordExpirationDays</span></span>|<span data-ttu-id="f731a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f731a-169">Int32</span></span>|<span data-ttu-id="f731a-170">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="f731a-170">The password expiration in days.</span></span>|
|<span data-ttu-id="f731a-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f731a-171">passwordMinimumLength</span></span>|<span data-ttu-id="f731a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f731a-172">Int32</span></span>|<span data-ttu-id="f731a-173">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f731a-173">The minimum password length.</span></span>|
|<span data-ttu-id="f731a-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f731a-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f731a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f731a-175">Int32</span></span>|<span data-ttu-id="f731a-176">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="f731a-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f731a-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f731a-177">passwordRequiredType</span></span>|[<span data-ttu-id="f731a-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f731a-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f731a-179">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="f731a-179">The required password type.</span></span> <span data-ttu-id="f731a-180">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f731a-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f731a-181">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f731a-181">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f731a-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f731a-182">Int32</span></span>|<span data-ttu-id="f731a-183">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="f731a-183">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="f731a-184">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="f731a-184">requireHealthyDeviceReport</span></span>|<span data-ttu-id="f731a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-185">Boolean</span></span>|<span data-ttu-id="f731a-186">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f731a-186">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f731a-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f731a-187">osMinimumVersion</span></span>|<span data-ttu-id="f731a-188">String</span><span class="sxs-lookup"><span data-stu-id="f731a-188">String</span></span>|<span data-ttu-id="f731a-189">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f731a-189">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="f731a-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f731a-190">osMaximumVersion</span></span>|<span data-ttu-id="f731a-191">String</span><span class="sxs-lookup"><span data-stu-id="f731a-191">String</span></span>|<span data-ttu-id="f731a-192">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f731a-192">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="f731a-193">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f731a-193">mobileOsMinimumVersion</span></span>|<span data-ttu-id="f731a-194">String</span><span class="sxs-lookup"><span data-stu-id="f731a-194">String</span></span>|<span data-ttu-id="f731a-195">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f731a-195">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f731a-196">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f731a-196">mobileOsMaximumVersion</span></span>|<span data-ttu-id="f731a-197">String</span><span class="sxs-lookup"><span data-stu-id="f731a-197">String</span></span>|<span data-ttu-id="f731a-198">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f731a-198">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f731a-199">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="f731a-199">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="f731a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-200">Boolean</span></span>|<span data-ttu-id="f731a-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="f731a-201">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="f731a-202">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="f731a-202">bitLockerEnabled</span></span>|<span data-ttu-id="f731a-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-203">Boolean</span></span>|<span data-ttu-id="f731a-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="f731a-204">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="f731a-205">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="f731a-205">secureBootEnabled</span></span>|<span data-ttu-id="f731a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-206">Boolean</span></span>|<span data-ttu-id="f731a-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="f731a-207">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="f731a-208">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="f731a-208">codeIntegrityEnabled</span></span>|<span data-ttu-id="f731a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-209">Boolean</span></span>|<span data-ttu-id="f731a-210">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="f731a-210">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f731a-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f731a-211">storageRequireEncryption</span></span>|<span data-ttu-id="f731a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f731a-212">Boolean</span></span>|<span data-ttu-id="f731a-213">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="f731a-213">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f731a-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="f731a-214">Response</span></span>
<span data-ttu-id="f731a-215">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f731a-215">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f731a-216">Пример</span><span class="sxs-lookup"><span data-stu-id="f731a-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="f731a-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="f731a-217">Request</span></span>
<span data-ttu-id="f731a-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f731a-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="f731a-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="f731a-219">Response</span></span>
<span data-ttu-id="f731a-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f731a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```




