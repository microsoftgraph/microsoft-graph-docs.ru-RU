---
title: Создание androidForWorkCompliancePolicy
description: Создайте новый объект AndroidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac3affaf984f252e51bcdcf8490dd8294217a6d5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665506"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="3b0e3-103">Создание androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3b0e3-103">Create androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="3b0e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b0e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b0e3-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b0e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b0e3-107">Создайте новый [объект AndroidForWorkCompliancePolicy.](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b0e3-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b0e3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b0e3-108">Prerequisites</span></span>
<span data-ttu-id="3b0e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b0e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b0e3-111">Permission type</span></span>|<span data-ttu-id="3b0e3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b0e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b0e3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b0e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b0e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b0e3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b0e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b0e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-116">Not supported.</span></span>|
|<span data-ttu-id="3b0e3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b0e3-117">Application</span></span>|<span data-ttu-id="3b0e3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0e3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b0e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b0e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3b0e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b0e3-120">Request headers</span></span>
|<span data-ttu-id="3b0e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b0e3-121">Header</span></span>|<span data-ttu-id="3b0e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b0e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b0e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b0e3-123">Authorization</span></span>|<span data-ttu-id="3b0e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b0e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b0e3-125">Accept</span></span>|<span data-ttu-id="3b0e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b0e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b0e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b0e3-127">Request body</span></span>
<span data-ttu-id="3b0e3-128">В теле запроса поставляем представление JSON для объекта AndroidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="3b0e3-129">В следующей таблице показаны свойства, необходимые при создании androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="3b0e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b0e3-130">Property</span></span>|<span data-ttu-id="3b0e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b0e3-131">Type</span></span>|<span data-ttu-id="3b0e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b0e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b0e3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b0e3-133">roleScopeTagIds</span></span>|<span data-ttu-id="3b0e3-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b0e3-134">String collection</span></span>|<span data-ttu-id="3b0e3-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3b0e3-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-137">id</span><span class="sxs-lookup"><span data-stu-id="3b0e3-137">id</span></span>|<span data-ttu-id="3b0e3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="3b0e3-138">String</span></span>|<span data-ttu-id="3b0e3-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-139">Key of the entity.</span></span> <span data-ttu-id="3b0e3-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0e3-141">createdDateTime</span></span>|<span data-ttu-id="3b0e3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0e3-142">DateTimeOffset</span></span>|<span data-ttu-id="3b0e3-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-143">DateTime the object was created.</span></span> <span data-ttu-id="3b0e3-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-145">description</span><span class="sxs-lookup"><span data-stu-id="3b0e3-145">description</span></span>|<span data-ttu-id="3b0e3-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3b0e3-146">String</span></span>|<span data-ttu-id="3b0e3-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b0e3-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0e3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="3b0e3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0e3-150">DateTimeOffset</span></span>|<span data-ttu-id="3b0e3-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="3b0e3-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3b0e3-153">displayName</span></span>|<span data-ttu-id="3b0e3-154">Строка</span><span class="sxs-lookup"><span data-stu-id="3b0e3-154">String</span></span>|<span data-ttu-id="3b0e3-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b0e3-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-157">version</span><span class="sxs-lookup"><span data-stu-id="3b0e3-157">version</span></span>|<span data-ttu-id="3b0e3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3b0e3-158">Int32</span></span>|<span data-ttu-id="3b0e3-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-159">Version of the device configuration.</span></span> <span data-ttu-id="3b0e3-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b0e3-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3b0e3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3b0e3-161">passwordRequired</span></span>|<span data-ttu-id="3b0e3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-162">Boolean</span></span>|<span data-ttu-id="3b0e3-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="3b0e3-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3b0e3-164">passwordMinimumLength</span></span>|<span data-ttu-id="3b0e3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3b0e3-165">Int32</span></span>|<span data-ttu-id="3b0e3-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-166">Minimum password length.</span></span> <span data-ttu-id="3b0e3-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3b0e3-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3b0e3-168">passwordRequiredType</span></span>|[<span data-ttu-id="3b0e3-169">AndroidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3b0e3-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="3b0e3-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-170">Type of characters in password.</span></span> <span data-ttu-id="3b0e3-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="3b0e3-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3b0e3-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3b0e3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3b0e3-173">Int32</span></span>|<span data-ttu-id="3b0e3-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3b0e3-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3b0e3-175">passwordExpirationDays</span></span>|<span data-ttu-id="3b0e3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3b0e3-176">Int32</span></span>|<span data-ttu-id="3b0e3-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-177">Number of days before the password expires.</span></span> <span data-ttu-id="3b0e3-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3b0e3-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3b0e3-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3b0e3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="3b0e3-180">Int32</span></span>|<span data-ttu-id="3b0e3-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-181">Number of previous passwords to block.</span></span> <span data-ttu-id="3b0e3-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3b0e3-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3b0e3-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3b0e3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3b0e3-184">Int32</span></span>|<span data-ttu-id="3b0e3-185">Количество отказов при входе, разрешенных до сброса завода.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="3b0e3-186">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="3b0e3-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3b0e3-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="3b0e3-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="3b0e3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-188">Boolean</span></span>|<span data-ttu-id="3b0e3-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="3b0e3-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="3b0e3-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="3b0e3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-191">Boolean</span></span>|<span data-ttu-id="3b0e3-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="3b0e3-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3b0e3-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="3b0e3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-194">Boolean</span></span>|<span data-ttu-id="3b0e3-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="3b0e3-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3b0e3-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3b0e3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-197">Boolean</span></span>|<span data-ttu-id="3b0e3-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="3b0e3-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3b0e3-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3b0e3-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3b0e3-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3b0e3-201">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3b0e3-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3b0e3-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="3b0e3-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="3b0e3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-204">Boolean</span></span>|<span data-ttu-id="3b0e3-205">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="3b0e3-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3b0e3-206">osMinimumVersion</span></span>|<span data-ttu-id="3b0e3-207">String</span><span class="sxs-lookup"><span data-stu-id="3b0e3-207">String</span></span>|<span data-ttu-id="3b0e3-208">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-208">Minimum Android version.</span></span>|
|<span data-ttu-id="3b0e3-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3b0e3-209">osMaximumVersion</span></span>|<span data-ttu-id="3b0e3-210">String</span><span class="sxs-lookup"><span data-stu-id="3b0e3-210">String</span></span>|<span data-ttu-id="3b0e3-211">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-211">Maximum Android version.</span></span>|
|<span data-ttu-id="3b0e3-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3b0e3-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="3b0e3-213">String</span><span class="sxs-lookup"><span data-stu-id="3b0e3-213">String</span></span>|<span data-ttu-id="3b0e3-214">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="3b0e3-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3b0e3-215">storageRequireEncryption</span></span>|<span data-ttu-id="3b0e3-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-216">Boolean</span></span>|<span data-ttu-id="3b0e3-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="3b0e3-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="3b0e3-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="3b0e3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-219">Boolean</span></span>|<span data-ttu-id="3b0e3-220">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="3b0e3-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="3b0e3-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="3b0e3-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-222">Boolean</span></span>|<span data-ttu-id="3b0e3-223">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="3b0e3-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="3b0e3-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="3b0e3-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-225">Boolean</span></span>|<span data-ttu-id="3b0e3-226">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="3b0e3-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="3b0e3-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="3b0e3-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-228">Boolean</span></span>|<span data-ttu-id="3b0e3-229">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="3b0e3-230">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="3b0e3-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="3b0e3-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="3b0e3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0e3-232">Boolean</span></span>|<span data-ttu-id="3b0e3-233">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="3b0e3-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="3b0e3-234">securityRequiredAndroidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="3b0e3-234">securityRequiredAndroidSafetyNetEvaluationType</span></span>|[<span data-ttu-id="3b0e3-235">AndroidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="3b0e3-235">androidSafetyNetEvaluationType</span></span>](../resources/intune-deviceconfig-androidsafetynetevaluationtype.md)|<span data-ttu-id="3b0e3-236">Требуется определенный тип оценки SafetyNet для соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-236">Require a specific SafetyNet evaluation type for compliance.</span></span> <span data-ttu-id="3b0e3-237">Возможные значения: `basic`, `hardwareBacked`.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-237">Possible values are: `basic`, `hardwareBacked`.</span></span>|



## <a name="response"></a><span data-ttu-id="3b0e3-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b0e3-238">Response</span></span>
<span data-ttu-id="3b0e3-239">В случае успешного использования этот метод возвращает код отклика и `201 Created` [объект AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-239">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b0e3-240">Пример</span><span class="sxs-lookup"><span data-stu-id="3b0e3-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b0e3-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b0e3-241">Request</span></span>
<span data-ttu-id="3b0e3-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```

### <a name="response"></a><span data-ttu-id="3b0e3-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b0e3-243">Response</span></span>
<span data-ttu-id="3b0e3-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b0e3-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1526

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```




