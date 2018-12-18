---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: d80bcd8852a21a1aac216fdee283fb6ba61b461e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333399"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="aec8e-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="aec8e-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="aec8e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aec8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aec8e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aec8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aec8e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aec8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aec8e-107">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aec8e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aec8e-108">Prerequisites</span></span>
<span data-ttu-id="aec8e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec8e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aec8e-111">Permission type</span></span>|<span data-ttu-id="aec8e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aec8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aec8e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aec8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aec8e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec8e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aec8e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aec8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aec8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aec8e-116">Not supported.</span></span>|
|<span data-ttu-id="aec8e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aec8e-117">Application</span></span>|<span data-ttu-id="aec8e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aec8e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aec8e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aec8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="aec8e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aec8e-120">Request headers</span></span>
|<span data-ttu-id="aec8e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aec8e-121">Header</span></span>|<span data-ttu-id="aec8e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aec8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aec8e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aec8e-123">Authorization</span></span>|<span data-ttu-id="aec8e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aec8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aec8e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aec8e-125">Accept</span></span>|<span data-ttu-id="aec8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aec8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec8e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aec8e-127">Request body</span></span>
<span data-ttu-id="aec8e-128">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aec8e-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="aec8e-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="aec8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aec8e-130">Property</span></span>|<span data-ttu-id="aec8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aec8e-131">Type</span></span>|<span data-ttu-id="aec8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aec8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec8e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aec8e-133">roleScopeTagIds</span></span>|<span data-ttu-id="aec8e-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aec8e-134">String collection</span></span>|<span data-ttu-id="aec8e-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="aec8e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aec8e-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-137">id</span><span class="sxs-lookup"><span data-stu-id="aec8e-137">id</span></span>|<span data-ttu-id="aec8e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="aec8e-138">String</span></span>|<span data-ttu-id="aec8e-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aec8e-139">Key of the entity.</span></span> <span data-ttu-id="aec8e-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aec8e-141">createdDateTime</span></span>|<span data-ttu-id="aec8e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec8e-142">DateTimeOffset</span></span>|<span data-ttu-id="aec8e-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aec8e-143">DateTime the object was created.</span></span> <span data-ttu-id="aec8e-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-145">описание</span><span class="sxs-lookup"><span data-stu-id="aec8e-145">description</span></span>|<span data-ttu-id="aec8e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="aec8e-146">String</span></span>|<span data-ttu-id="aec8e-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aec8e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aec8e-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aec8e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="aec8e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec8e-150">DateTimeOffset</span></span>|<span data-ttu-id="aec8e-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aec8e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="aec8e-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="aec8e-153">displayName</span></span>|<span data-ttu-id="aec8e-154">Строка</span><span class="sxs-lookup"><span data-stu-id="aec8e-154">String</span></span>|<span data-ttu-id="aec8e-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aec8e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aec8e-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-157">version</span><span class="sxs-lookup"><span data-stu-id="aec8e-157">version</span></span>|<span data-ttu-id="aec8e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aec8e-158">Int32</span></span>|<span data-ttu-id="aec8e-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aec8e-159">Version of the device configuration.</span></span> <span data-ttu-id="aec8e-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aec8e-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aec8e-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aec8e-161">passwordRequired</span></span>|<span data-ttu-id="aec8e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-162">Boolean</span></span>|<span data-ttu-id="aec8e-163">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="aec8e-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="aec8e-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="aec8e-164">passwordBlockSimple</span></span>|<span data-ttu-id="aec8e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-165">Boolean</span></span>|<span data-ttu-id="aec8e-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="aec8e-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="aec8e-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="aec8e-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="aec8e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-168">Boolean</span></span>|<span data-ttu-id="aec8e-169">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="aec8e-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="aec8e-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="aec8e-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="aec8e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="aec8e-171">Int32</span></span>|<span data-ttu-id="aec8e-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="aec8e-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="aec8e-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aec8e-173">passwordExpirationDays</span></span>|<span data-ttu-id="aec8e-174">Int32</span><span class="sxs-lookup"><span data-stu-id="aec8e-174">Int32</span></span>|<span data-ttu-id="aec8e-175">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="aec8e-175">The password expiration in days.</span></span>|
|<span data-ttu-id="aec8e-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aec8e-176">passwordMinimumLength</span></span>|<span data-ttu-id="aec8e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aec8e-177">Int32</span></span>|<span data-ttu-id="aec8e-178">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="aec8e-178">The minimum password length.</span></span>|
|<span data-ttu-id="aec8e-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="aec8e-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="aec8e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="aec8e-180">Int32</span></span>|<span data-ttu-id="aec8e-181">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="aec8e-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="aec8e-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aec8e-182">passwordRequiredType</span></span>|[<span data-ttu-id="aec8e-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aec8e-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="aec8e-184">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="aec8e-184">The required password type.</span></span> <span data-ttu-id="aec8e-185">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="aec8e-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="aec8e-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aec8e-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aec8e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="aec8e-187">Int32</span></span>|<span data-ttu-id="aec8e-188">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="aec8e-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="aec8e-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="aec8e-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="aec8e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-190">Boolean</span></span>|<span data-ttu-id="aec8e-191">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="aec8e-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="aec8e-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aec8e-192">osMinimumVersion</span></span>|<span data-ttu-id="aec8e-193">String</span><span class="sxs-lookup"><span data-stu-id="aec8e-193">String</span></span>|<span data-ttu-id="aec8e-194">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aec8e-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="aec8e-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aec8e-195">osMaximumVersion</span></span>|<span data-ttu-id="aec8e-196">String</span><span class="sxs-lookup"><span data-stu-id="aec8e-196">String</span></span>|<span data-ttu-id="aec8e-197">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aec8e-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="aec8e-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aec8e-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="aec8e-199">String</span><span class="sxs-lookup"><span data-stu-id="aec8e-199">String</span></span>|<span data-ttu-id="aec8e-200">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aec8e-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="aec8e-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aec8e-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="aec8e-202">String</span><span class="sxs-lookup"><span data-stu-id="aec8e-202">String</span></span>|<span data-ttu-id="aec8e-203">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aec8e-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="aec8e-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="aec8e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-205">Boolean</span></span>|<span data-ttu-id="aec8e-206">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="aec8e-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="aec8e-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-207">bitLockerEnabled</span></span>|<span data-ttu-id="aec8e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-208">Boolean</span></span>|<span data-ttu-id="aec8e-209">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="aec8e-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="aec8e-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-210">secureBootEnabled</span></span>|<span data-ttu-id="aec8e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-211">Boolean</span></span>|<span data-ttu-id="aec8e-212">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="aec8e-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="aec8e-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="aec8e-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-214">Boolean</span></span>|<span data-ttu-id="aec8e-215">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="aec8e-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="aec8e-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="aec8e-216">storageRequireEncryption</span></span>|<span data-ttu-id="aec8e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-217">Boolean</span></span>|<span data-ttu-id="aec8e-218">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="aec8e-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="aec8e-219">activeFirewallRequired</span></span>|<span data-ttu-id="aec8e-220">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-220">Boolean</span></span>|<span data-ttu-id="aec8e-221">Требуется active брандмауэра на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="aec8e-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-222">defenderEnabled</span></span>|<span data-ttu-id="aec8e-223">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-223">Boolean</span></span>|<span data-ttu-id="aec8e-224">Требуется Защитник Windows защиты от вредоносных программ на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="aec8e-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="aec8e-225">defenderVersion</span></span>|<span data-ttu-id="aec8e-226">String.</span><span class="sxs-lookup"><span data-stu-id="aec8e-226">String</span></span>|<span data-ttu-id="aec8e-227">Требуется Минимальная версия Защитника Windows защиты от вредоносных программ на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="aec8e-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="aec8e-228">signatureOutOfDate</span></span>|<span data-ttu-id="aec8e-229">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-229">Boolean</span></span>|<span data-ttu-id="aec8e-230">Требование подписи защиты от вредоносных программ Защитника Windows быть в курсе устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="aec8e-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-231">rtpEnabled</span></span>|<span data-ttu-id="aec8e-232">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-232">Boolean</span></span>|<span data-ttu-id="aec8e-233">Требовать защиту в реальном времени защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="aec8e-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="aec8e-234">antivirusRequired</span></span>|<span data-ttu-id="aec8e-235">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-235">Boolean</span></span>|<span data-ttu-id="aec8e-236">Требуется антивирусное решение, зарегистрированных в центр Decurity Windows должна находиться на и мониторинг (например Symantec, Защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="aec8e-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="aec8e-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="aec8e-237">antiSpywareRequired</span></span>|<span data-ttu-id="aec8e-238">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-238">Boolean</span></span>|<span data-ttu-id="aec8e-239">Требуется любой антишпионское решение, зарегистрированные с центром Decurity Windows должна находиться на и мониторинг (например, Symantec, Защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="aec8e-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="aec8e-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="aec8e-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="aec8e-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="aec8e-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="aec8e-242">Допустимый операционной системы выполните построение диапазонов на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="aec8e-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="aec8e-243">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="aec8e-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="aec8e-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="aec8e-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="aec8e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec8e-245">Boolean</span></span>|<span data-ttu-id="aec8e-246">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="aec8e-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="aec8e-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="aec8e-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="aec8e-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="aec8e-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="aec8e-249">Требовать защиту от угроз устройства минимальным риском и сообщение о несовместимости.</span><span class="sxs-lookup"><span data-stu-id="aec8e-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="aec8e-250">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="aec8e-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="aec8e-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="aec8e-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="aec8e-252">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aec8e-252">Boolean</span></span>|<span data-ttu-id="aec8e-253">Требовать необходимо рассмотреть состояние соответствия SCCM во внимание для состояния Intune соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="aec8e-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="aec8e-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="aec8e-254">Response</span></span>
<span data-ttu-id="aec8e-255">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aec8e-255">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aec8e-256">Пример</span><span class="sxs-lookup"><span data-stu-id="aec8e-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="aec8e-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="aec8e-257">Request</span></span>
<span data-ttu-id="aec8e-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aec8e-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="aec8e-259">Ответ</span><span class="sxs-lookup"><span data-stu-id="aec8e-259">Response</span></span>
<span data-ttu-id="aec8e-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aec8e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

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
  "configurationManagerComplianceRequired": true
}
```





