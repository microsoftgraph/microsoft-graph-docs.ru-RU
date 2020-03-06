---
title: Создание androidWorkProfileGeneralDeviceConfiguration
description: Создание нового объекта androidWorkProfileGeneralDeviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86a0c8a5951d22a5283d5343201a2efa7d85ca64
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515226"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="ccc53-103">Создание androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ccc53-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="ccc53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccc53-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccc53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc53-106">Создание нового объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ccc53-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccc53-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ccc53-107">Prerequisites</span></span>
<span data-ttu-id="ccc53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccc53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc53-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc53-110">Permission type</span></span>|<span data-ttu-id="ccc53-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccc53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccc53-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccc53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccc53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccc53-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccc53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc53-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccc53-115">Not supported.</span></span>|
|<span data-ttu-id="ccc53-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccc53-116">Application</span></span>|<span data-ttu-id="ccc53-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccc53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc53-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccc53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ccc53-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ccc53-119">Request headers</span></span>
|<span data-ttu-id="ccc53-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccc53-120">Header</span></span>|<span data-ttu-id="ccc53-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ccc53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccc53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc53-122">Authorization</span></span>|<span data-ttu-id="ccc53-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccc53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccc53-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ccc53-124">Accept</span></span>|<span data-ttu-id="ccc53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ccc53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc53-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccc53-126">Request body</span></span>
<span data-ttu-id="ccc53-127">В тексте запроса добавьте представление объекта androidWorkProfileGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccc53-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="ccc53-128">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ccc53-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="ccc53-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccc53-129">Property</span></span>|<span data-ttu-id="ccc53-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ccc53-130">Type</span></span>|<span data-ttu-id="ccc53-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc53-132">id</span><span class="sxs-lookup"><span data-stu-id="ccc53-132">id</span></span>|<span data-ttu-id="ccc53-133">String</span><span class="sxs-lookup"><span data-stu-id="ccc53-133">String</span></span>|<span data-ttu-id="ccc53-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ccc53-134">Key of the entity.</span></span> <span data-ttu-id="ccc53-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccc53-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccc53-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccc53-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ccc53-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccc53-137">DateTimeOffset</span></span>|<span data-ttu-id="ccc53-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ccc53-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ccc53-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccc53-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccc53-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccc53-140">createdDateTime</span></span>|<span data-ttu-id="ccc53-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccc53-141">DateTimeOffset</span></span>|<span data-ttu-id="ccc53-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ccc53-142">DateTime the object was created.</span></span> <span data-ttu-id="ccc53-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccc53-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccc53-144">description</span><span class="sxs-lookup"><span data-stu-id="ccc53-144">description</span></span>|<span data-ttu-id="ccc53-145">String</span><span class="sxs-lookup"><span data-stu-id="ccc53-145">String</span></span>|<span data-ttu-id="ccc53-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccc53-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ccc53-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccc53-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccc53-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ccc53-148">displayName</span></span>|<span data-ttu-id="ccc53-149">Строка</span><span class="sxs-lookup"><span data-stu-id="ccc53-149">String</span></span>|<span data-ttu-id="ccc53-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccc53-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ccc53-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccc53-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccc53-152">version</span><span class="sxs-lookup"><span data-stu-id="ccc53-152">version</span></span>|<span data-ttu-id="ccc53-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-153">Int32</span></span>|<span data-ttu-id="ccc53-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccc53-154">Version of the device configuration.</span></span> <span data-ttu-id="ccc53-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccc53-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccc53-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ccc53-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="ccc53-157">Логический</span><span class="sxs-lookup"><span data-stu-id="ccc53-157">Boolean</span></span>|<span data-ttu-id="ccc53-158">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="ccc53-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ccc53-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="ccc53-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="ccc53-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-160">Boolean</span></span>|<span data-ttu-id="ccc53-161">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="ccc53-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="ccc53-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ccc53-162">passwordExpirationDays</span></span>|<span data-ttu-id="ccc53-163">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-163">Int32</span></span>|<span data-ttu-id="ccc53-164">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-164">Number of days before the password expires.</span></span> <span data-ttu-id="ccc53-165">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="ccc53-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ccc53-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ccc53-166">passwordMinimumLength</span></span>|<span data-ttu-id="ccc53-167">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-167">Int32</span></span>|<span data-ttu-id="ccc53-168">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="ccc53-168">Minimum length of passwords.</span></span> <span data-ttu-id="ccc53-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="ccc53-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ccc53-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ccc53-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ccc53-171">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-171">Int32</span></span>|<span data-ttu-id="ccc53-172">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ccc53-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ccc53-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ccc53-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ccc53-174">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-174">Int32</span></span>|<span data-ttu-id="ccc53-175">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="ccc53-175">Number of previous passwords to block.</span></span> <span data-ttu-id="ccc53-176">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="ccc53-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ccc53-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ccc53-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ccc53-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-178">Int32</span></span>|<span data-ttu-id="ccc53-179">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="ccc53-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="ccc53-180">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="ccc53-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ccc53-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ccc53-181">passwordRequiredType</span></span>|[<span data-ttu-id="ccc53-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ccc53-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="ccc53-183">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-183">Type of password that is required.</span></span> <span data-ttu-id="ccc53-184">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="ccc53-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="ccc53-185">воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="ccc53-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="ccc53-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="ccc53-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="ccc53-187">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="ccc53-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="ccc53-188">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="ccc53-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="ccc53-189">воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="ccc53-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="ccc53-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-190">Boolean</span></span>|<span data-ttu-id="ccc53-191">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="ccc53-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="ccc53-192">воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="ccc53-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="ccc53-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-193">Boolean</span></span>|<span data-ttu-id="ccc53-194">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="ccc53-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="ccc53-195">воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="ccc53-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="ccc53-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-196">Boolean</span></span>|<span data-ttu-id="ccc53-197">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="ccc53-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="ccc53-198">воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="ccc53-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="ccc53-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-199">Boolean</span></span>|<span data-ttu-id="ccc53-200">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="ccc53-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="ccc53-201">воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="ccc53-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="ccc53-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-202">Boolean</span></span>|<span data-ttu-id="ccc53-203">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="ccc53-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="ccc53-204">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="ccc53-204">workProfileBlockCamera</span></span>|<span data-ttu-id="ccc53-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-205">Boolean</span></span>|<span data-ttu-id="ccc53-206">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-206">Block work profile camera.</span></span>|
|<span data-ttu-id="ccc53-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="ccc53-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="ccc53-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-208">Boolean</span></span>|<span data-ttu-id="ccc53-209">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="ccc53-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="ccc53-210">воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="ccc53-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="ccc53-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-211">Boolean</span></span>|<span data-ttu-id="ccc53-212">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="ccc53-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="ccc53-213">воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="ccc53-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="ccc53-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="ccc53-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="ccc53-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-215">Type of password that is required.</span></span> <span data-ttu-id="ccc53-216">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="ccc53-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="ccc53-217">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="ccc53-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="ccc53-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-218">Boolean</span></span>|<span data-ttu-id="ccc53-219">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="ccc53-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="ccc53-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="ccc53-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-221">Boolean</span></span>|<span data-ttu-id="ccc53-222">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="ccc53-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="ccc53-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ccc53-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="ccc53-224">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-224">Int32</span></span>|<span data-ttu-id="ccc53-225">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="ccc53-226">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="ccc53-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ccc53-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ccc53-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="ccc53-228">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-228">Int32</span></span>|<span data-ttu-id="ccc53-229">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-229">Minimum length of work profile password.</span></span> <span data-ttu-id="ccc53-230">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="ccc53-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ccc53-231">воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="ccc53-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="ccc53-232">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-232">Int32</span></span>|<span data-ttu-id="ccc53-233">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="ccc53-234">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="ccc53-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="ccc53-235">воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="ccc53-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="ccc53-236">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-236">Int32</span></span>|<span data-ttu-id="ccc53-237">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="ccc53-238">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="ccc53-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="ccc53-239">воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="ccc53-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="ccc53-240">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-240">Int32</span></span>|<span data-ttu-id="ccc53-241">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="ccc53-242">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="ccc53-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="ccc53-243">воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="ccc53-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="ccc53-244">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-244">Int32</span></span>|<span data-ttu-id="ccc53-245">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="ccc53-246">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="ccc53-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="ccc53-247">воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="ccc53-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="ccc53-248">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-248">Int32</span></span>|<span data-ttu-id="ccc53-249">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="ccc53-250">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="ccc53-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="ccc53-251">воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="ccc53-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="ccc53-252">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-252">Int32</span></span>|<span data-ttu-id="ccc53-253">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="ccc53-254">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="ccc53-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="ccc53-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ccc53-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ccc53-256">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-256">Int32</span></span>|<span data-ttu-id="ccc53-257">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ccc53-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ccc53-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ccc53-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ccc53-259">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-259">Int32</span></span>|<span data-ttu-id="ccc53-260">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="ccc53-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="ccc53-261">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="ccc53-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ccc53-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ccc53-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ccc53-263">Int32</span><span class="sxs-lookup"><span data-stu-id="ccc53-263">Int32</span></span>|<span data-ttu-id="ccc53-264">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="ccc53-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="ccc53-265">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="ccc53-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ccc53-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ccc53-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="ccc53-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ccc53-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="ccc53-268">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="ccc53-268">Type of work profile password that is required.</span></span> <span data-ttu-id="ccc53-269">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="ccc53-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="ccc53-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ccc53-270">workProfileRequirePassword</span></span>|<span data-ttu-id="ccc53-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-271">Boolean</span></span>|<span data-ttu-id="ccc53-272">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="ccc53-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="ccc53-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="ccc53-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="ccc53-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccc53-274">Boolean</span></span>|<span data-ttu-id="ccc53-275">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="ccc53-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="ccc53-276">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccc53-276">Response</span></span>
<span data-ttu-id="ccc53-277">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccc53-277">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccc53-278">Пример</span><span class="sxs-lookup"><span data-stu-id="ccc53-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccc53-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc53-279">Request</span></span>
<span data-ttu-id="ccc53-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccc53-280">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ccc53-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc53-281">Response</span></span>
<span data-ttu-id="ccc53-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccc53-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




