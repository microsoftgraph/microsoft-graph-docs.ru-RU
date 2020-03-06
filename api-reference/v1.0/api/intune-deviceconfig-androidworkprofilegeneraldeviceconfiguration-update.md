---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойств объекта androidWorkProfileGeneralDeviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6968e62a3c1fb3e86dc4329e569cea5eeda4722
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515198"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="dd7ad-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd7ad-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="dd7ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd7ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd7ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd7ad-106">Обновление свойств объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dd7ad-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd7ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd7ad-107">Prerequisites</span></span>
<span data-ttu-id="dd7ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd7ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7ad-110">Permission type</span></span>|<span data-ttu-id="dd7ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd7ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd7ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd7ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd7ad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd7ad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd7ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd7ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd7ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-115">Not supported.</span></span>|
|<span data-ttu-id="dd7ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd7ad-116">Application</span></span>|<span data-ttu-id="dd7ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd7ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd7ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dd7ad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd7ad-119">Request headers</span></span>
|<span data-ttu-id="dd7ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd7ad-120">Header</span></span>|<span data-ttu-id="dd7ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd7ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd7ad-122">Authorization</span></span>|<span data-ttu-id="dd7ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd7ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dd7ad-124">Accept</span></span>|<span data-ttu-id="dd7ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd7ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd7ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd7ad-126">Request body</span></span>
<span data-ttu-id="dd7ad-127">В тексте запроса добавьте представление объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="dd7ad-128">В следующей таблице приведены свойства, необходимые при создании [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="dd7ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7ad-129">Property</span></span>|<span data-ttu-id="dd7ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7ad-130">Type</span></span>|<span data-ttu-id="dd7ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dd7ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd7ad-132">id</span><span class="sxs-lookup"><span data-stu-id="dd7ad-132">id</span></span>|<span data-ttu-id="dd7ad-133">String</span><span class="sxs-lookup"><span data-stu-id="dd7ad-133">String</span></span>|<span data-ttu-id="dd7ad-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-134">Key of the entity.</span></span> <span data-ttu-id="dd7ad-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd7ad-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7ad-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dd7ad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7ad-137">DateTimeOffset</span></span>|<span data-ttu-id="dd7ad-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dd7ad-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd7ad-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7ad-140">createdDateTime</span></span>|<span data-ttu-id="dd7ad-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7ad-141">DateTimeOffset</span></span>|<span data-ttu-id="dd7ad-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-142">DateTime the object was created.</span></span> <span data-ttu-id="dd7ad-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd7ad-144">description</span><span class="sxs-lookup"><span data-stu-id="dd7ad-144">description</span></span>|<span data-ttu-id="dd7ad-145">String</span><span class="sxs-lookup"><span data-stu-id="dd7ad-145">String</span></span>|<span data-ttu-id="dd7ad-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd7ad-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd7ad-148">displayName</span><span class="sxs-lookup"><span data-stu-id="dd7ad-148">displayName</span></span>|<span data-ttu-id="dd7ad-149">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7ad-149">String</span></span>|<span data-ttu-id="dd7ad-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd7ad-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd7ad-152">version</span><span class="sxs-lookup"><span data-stu-id="dd7ad-152">version</span></span>|<span data-ttu-id="dd7ad-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-153">Int32</span></span>|<span data-ttu-id="dd7ad-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-154">Version of the device configuration.</span></span> <span data-ttu-id="dd7ad-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd7ad-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="dd7ad-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="dd7ad-157">Логический</span><span class="sxs-lookup"><span data-stu-id="dd7ad-157">Boolean</span></span>|<span data-ttu-id="dd7ad-158">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="dd7ad-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="dd7ad-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="dd7ad-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-160">Boolean</span></span>|<span data-ttu-id="dd7ad-161">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="dd7ad-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dd7ad-162">passwordExpirationDays</span></span>|<span data-ttu-id="dd7ad-163">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-163">Int32</span></span>|<span data-ttu-id="dd7ad-164">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-164">Number of days before the password expires.</span></span> <span data-ttu-id="dd7ad-165">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="dd7ad-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dd7ad-166">passwordMinimumLength</span></span>|<span data-ttu-id="dd7ad-167">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-167">Int32</span></span>|<span data-ttu-id="dd7ad-168">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-168">Minimum length of passwords.</span></span> <span data-ttu-id="dd7ad-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="dd7ad-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dd7ad-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dd7ad-171">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-171">Int32</span></span>|<span data-ttu-id="dd7ad-172">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="dd7ad-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dd7ad-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dd7ad-174">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-174">Int32</span></span>|<span data-ttu-id="dd7ad-175">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-175">Number of previous passwords to block.</span></span> <span data-ttu-id="dd7ad-176">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dd7ad-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="dd7ad-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="dd7ad-178">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-178">Int32</span></span>|<span data-ttu-id="dd7ad-179">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="dd7ad-180">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="dd7ad-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dd7ad-181">passwordRequiredType</span></span>|[<span data-ttu-id="dd7ad-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dd7ad-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="dd7ad-183">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-183">Type of password that is required.</span></span> <span data-ttu-id="dd7ad-184">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="dd7ad-185">воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="dd7ad-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="dd7ad-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="dd7ad-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="dd7ad-187">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="dd7ad-188">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="dd7ad-189">воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="dd7ad-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="dd7ad-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-190">Boolean</span></span>|<span data-ttu-id="dd7ad-191">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="dd7ad-192">воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="dd7ad-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-193">Boolean</span></span>|<span data-ttu-id="dd7ad-194">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="dd7ad-195">воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="dd7ad-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="dd7ad-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-196">Boolean</span></span>|<span data-ttu-id="dd7ad-197">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="dd7ad-198">воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="dd7ad-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="dd7ad-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-199">Boolean</span></span>|<span data-ttu-id="dd7ad-200">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="dd7ad-201">воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="dd7ad-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="dd7ad-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-202">Boolean</span></span>|<span data-ttu-id="dd7ad-203">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="dd7ad-204">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="dd7ad-204">workProfileBlockCamera</span></span>|<span data-ttu-id="dd7ad-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-205">Boolean</span></span>|<span data-ttu-id="dd7ad-206">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-206">Block work profile camera.</span></span>|
|<span data-ttu-id="dd7ad-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="dd7ad-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="dd7ad-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-208">Boolean</span></span>|<span data-ttu-id="dd7ad-209">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="dd7ad-210">воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="dd7ad-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="dd7ad-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-211">Boolean</span></span>|<span data-ttu-id="dd7ad-212">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="dd7ad-213">воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="dd7ad-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="dd7ad-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="dd7ad-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="dd7ad-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-215">Type of password that is required.</span></span> <span data-ttu-id="dd7ad-216">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="dd7ad-217">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="dd7ad-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="dd7ad-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-218">Boolean</span></span>|<span data-ttu-id="dd7ad-219">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="dd7ad-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="dd7ad-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="dd7ad-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-221">Boolean</span></span>|<span data-ttu-id="dd7ad-222">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="dd7ad-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dd7ad-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="dd7ad-224">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-224">Int32</span></span>|<span data-ttu-id="dd7ad-225">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="dd7ad-226">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="dd7ad-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dd7ad-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="dd7ad-228">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-228">Int32</span></span>|<span data-ttu-id="dd7ad-229">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-229">Minimum length of work profile password.</span></span> <span data-ttu-id="dd7ad-230">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="dd7ad-231">воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="dd7ad-232">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-232">Int32</span></span>|<span data-ttu-id="dd7ad-233">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="dd7ad-234">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="dd7ad-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dd7ad-235">воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="dd7ad-236">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-236">Int32</span></span>|<span data-ttu-id="dd7ad-237">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="dd7ad-238">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="dd7ad-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dd7ad-239">воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="dd7ad-240">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-240">Int32</span></span>|<span data-ttu-id="dd7ad-241">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="dd7ad-242">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="dd7ad-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dd7ad-243">воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="dd7ad-244">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-244">Int32</span></span>|<span data-ttu-id="dd7ad-245">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="dd7ad-246">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="dd7ad-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dd7ad-247">воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="dd7ad-248">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-248">Int32</span></span>|<span data-ttu-id="dd7ad-249">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="dd7ad-250">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="dd7ad-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dd7ad-251">воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="dd7ad-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="dd7ad-252">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-252">Int32</span></span>|<span data-ttu-id="dd7ad-253">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="dd7ad-254">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="dd7ad-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dd7ad-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dd7ad-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dd7ad-256">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-256">Int32</span></span>|<span data-ttu-id="dd7ad-257">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="dd7ad-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="dd7ad-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dd7ad-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dd7ad-259">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-259">Int32</span></span>|<span data-ttu-id="dd7ad-260">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="dd7ad-261">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dd7ad-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="dd7ad-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="dd7ad-263">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7ad-263">Int32</span></span>|<span data-ttu-id="dd7ad-264">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="dd7ad-265">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="dd7ad-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dd7ad-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="dd7ad-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dd7ad-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="dd7ad-268">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-268">Type of work profile password that is required.</span></span> <span data-ttu-id="dd7ad-269">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="dd7ad-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="dd7ad-270">workProfileRequirePassword</span></span>|<span data-ttu-id="dd7ad-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-271">Boolean</span></span>|<span data-ttu-id="dd7ad-272">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="dd7ad-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="dd7ad-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="dd7ad-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="dd7ad-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd7ad-274">Boolean</span></span>|<span data-ttu-id="dd7ad-275">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="dd7ad-276">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7ad-276">Response</span></span>
<span data-ttu-id="dd7ad-277">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-277">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd7ad-278">Пример</span><span class="sxs-lookup"><span data-stu-id="dd7ad-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd7ad-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7ad-279">Request</span></span>
<span data-ttu-id="dd7ad-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="dd7ad-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd7ad-281">Response</span></span>
<span data-ttu-id="dd7ad-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd7ad-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```




