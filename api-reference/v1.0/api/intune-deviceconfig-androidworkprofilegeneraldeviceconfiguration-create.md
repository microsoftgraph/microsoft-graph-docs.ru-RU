---
title: Создание androidWorkProfileGeneralDeviceConfiguration
description: Создание нового объекта androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cbdbbfd5881369add35b89149fdef1fdadab2f9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401155"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="369f6-103">Создание androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="369f6-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="369f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="369f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="369f6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="369f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="369f6-106">Создание нового объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="369f6-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="369f6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="369f6-107">Prerequisites</span></span>
<span data-ttu-id="369f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="369f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="369f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="369f6-110">Permission type</span></span>|<span data-ttu-id="369f6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="369f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="369f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="369f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="369f6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="369f6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="369f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="369f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="369f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="369f6-115">Not supported.</span></span>|
|<span data-ttu-id="369f6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="369f6-116">Application</span></span>|<span data-ttu-id="369f6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="369f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="369f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="369f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="369f6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="369f6-119">Request headers</span></span>
|<span data-ttu-id="369f6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="369f6-120">Header</span></span>|<span data-ttu-id="369f6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="369f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="369f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="369f6-122">Authorization</span></span>|<span data-ttu-id="369f6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="369f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="369f6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="369f6-124">Accept</span></span>|<span data-ttu-id="369f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="369f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="369f6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="369f6-126">Request body</span></span>
<span data-ttu-id="369f6-127">В тексте запроса добавьте представление объекта androidWorkProfileGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="369f6-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="369f6-128">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="369f6-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="369f6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="369f6-129">Property</span></span>|<span data-ttu-id="369f6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="369f6-130">Type</span></span>|<span data-ttu-id="369f6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="369f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="369f6-132">id</span><span class="sxs-lookup"><span data-stu-id="369f6-132">id</span></span>|<span data-ttu-id="369f6-133">String</span><span class="sxs-lookup"><span data-stu-id="369f6-133">String</span></span>|<span data-ttu-id="369f6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="369f6-134">Key of the entity.</span></span> <span data-ttu-id="369f6-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="369f6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="369f6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="369f6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="369f6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="369f6-137">DateTimeOffset</span></span>|<span data-ttu-id="369f6-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="369f6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="369f6-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="369f6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="369f6-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="369f6-140">createdDateTime</span></span>|<span data-ttu-id="369f6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="369f6-141">DateTimeOffset</span></span>|<span data-ttu-id="369f6-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="369f6-142">DateTime the object was created.</span></span> <span data-ttu-id="369f6-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="369f6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="369f6-144">description</span><span class="sxs-lookup"><span data-stu-id="369f6-144">description</span></span>|<span data-ttu-id="369f6-145">String</span><span class="sxs-lookup"><span data-stu-id="369f6-145">String</span></span>|<span data-ttu-id="369f6-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="369f6-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="369f6-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="369f6-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="369f6-148">displayName</span><span class="sxs-lookup"><span data-stu-id="369f6-148">displayName</span></span>|<span data-ttu-id="369f6-149">Строка</span><span class="sxs-lookup"><span data-stu-id="369f6-149">String</span></span>|<span data-ttu-id="369f6-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="369f6-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="369f6-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="369f6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="369f6-152">version</span><span class="sxs-lookup"><span data-stu-id="369f6-152">version</span></span>|<span data-ttu-id="369f6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-153">Int32</span></span>|<span data-ttu-id="369f6-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="369f6-154">Version of the device configuration.</span></span> <span data-ttu-id="369f6-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="369f6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="369f6-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="369f6-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="369f6-157">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-157">Boolean</span></span>|<span data-ttu-id="369f6-158">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="369f6-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="369f6-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="369f6-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="369f6-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="369f6-160">Boolean</span></span>|<span data-ttu-id="369f6-161">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="369f6-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="369f6-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="369f6-162">passwordExpirationDays</span></span>|<span data-ttu-id="369f6-163">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-163">Int32</span></span>|<span data-ttu-id="369f6-164">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="369f6-164">Number of days before the password expires.</span></span> <span data-ttu-id="369f6-165">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="369f6-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="369f6-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="369f6-166">passwordMinimumLength</span></span>|<span data-ttu-id="369f6-167">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-167">Int32</span></span>|<span data-ttu-id="369f6-168">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="369f6-168">Minimum length of passwords.</span></span> <span data-ttu-id="369f6-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="369f6-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="369f6-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="369f6-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="369f6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-171">Int32</span></span>|<span data-ttu-id="369f6-172">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="369f6-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="369f6-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="369f6-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="369f6-174">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-174">Int32</span></span>|<span data-ttu-id="369f6-175">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="369f6-175">Number of previous passwords to block.</span></span> <span data-ttu-id="369f6-176">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="369f6-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="369f6-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="369f6-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="369f6-178">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-178">Int32</span></span>|<span data-ttu-id="369f6-179">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="369f6-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="369f6-180">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="369f6-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="369f6-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="369f6-181">passwordRequiredType</span></span>|[<span data-ttu-id="369f6-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="369f6-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="369f6-183">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="369f6-183">Type of password that is required.</span></span> <span data-ttu-id="369f6-184">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="369f6-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="369f6-185">воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="369f6-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="369f6-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="369f6-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="369f6-187">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="369f6-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="369f6-188">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="369f6-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="369f6-189">воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="369f6-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="369f6-190">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-190">Boolean</span></span>|<span data-ttu-id="369f6-191">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="369f6-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="369f6-192">воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="369f6-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="369f6-193">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-193">Boolean</span></span>|<span data-ttu-id="369f6-194">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="369f6-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="369f6-195">воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="369f6-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="369f6-196">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-196">Boolean</span></span>|<span data-ttu-id="369f6-197">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="369f6-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="369f6-198">воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="369f6-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="369f6-199">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-199">Boolean</span></span>|<span data-ttu-id="369f6-200">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="369f6-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="369f6-201">воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="369f6-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="369f6-202">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-202">Boolean</span></span>|<span data-ttu-id="369f6-203">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="369f6-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="369f6-204">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="369f6-204">workProfileBlockCamera</span></span>|<span data-ttu-id="369f6-205">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-205">Boolean</span></span>|<span data-ttu-id="369f6-206">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-206">Block work profile camera.</span></span>|
|<span data-ttu-id="369f6-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="369f6-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="369f6-208">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-208">Boolean</span></span>|<span data-ttu-id="369f6-209">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="369f6-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="369f6-210">воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="369f6-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="369f6-211">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-211">Boolean</span></span>|<span data-ttu-id="369f6-212">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="369f6-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="369f6-213">воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="369f6-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="369f6-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="369f6-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="369f6-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="369f6-215">Type of password that is required.</span></span> <span data-ttu-id="369f6-216">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="369f6-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="369f6-217">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="369f6-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="369f6-218">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-218">Boolean</span></span>|<span data-ttu-id="369f6-219">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="369f6-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="369f6-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="369f6-221">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-221">Boolean</span></span>|<span data-ttu-id="369f6-222">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="369f6-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="369f6-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="369f6-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="369f6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-224">Int32</span></span>|<span data-ttu-id="369f6-225">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="369f6-226">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="369f6-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="369f6-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="369f6-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="369f6-228">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-228">Int32</span></span>|<span data-ttu-id="369f6-229">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-229">Minimum length of work profile password.</span></span> <span data-ttu-id="369f6-230">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="369f6-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="369f6-231">воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="369f6-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="369f6-232">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-232">Int32</span></span>|<span data-ttu-id="369f6-233">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="369f6-234">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="369f6-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="369f6-235">воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="369f6-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="369f6-236">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-236">Int32</span></span>|<span data-ttu-id="369f6-237">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="369f6-238">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="369f6-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="369f6-239">воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="369f6-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="369f6-240">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-240">Int32</span></span>|<span data-ttu-id="369f6-241">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="369f6-242">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="369f6-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="369f6-243">воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="369f6-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="369f6-244">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-244">Int32</span></span>|<span data-ttu-id="369f6-245">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="369f6-246">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="369f6-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="369f6-247">воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="369f6-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="369f6-248">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-248">Int32</span></span>|<span data-ttu-id="369f6-249">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="369f6-250">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="369f6-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="369f6-251">воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="369f6-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="369f6-252">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-252">Int32</span></span>|<span data-ttu-id="369f6-253">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="369f6-254">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="369f6-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="369f6-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="369f6-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="369f6-256">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-256">Int32</span></span>|<span data-ttu-id="369f6-257">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="369f6-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="369f6-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="369f6-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="369f6-259">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-259">Int32</span></span>|<span data-ttu-id="369f6-260">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="369f6-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="369f6-261">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="369f6-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="369f6-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="369f6-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="369f6-263">Int32</span><span class="sxs-lookup"><span data-stu-id="369f6-263">Int32</span></span>|<span data-ttu-id="369f6-264">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="369f6-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="369f6-265">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="369f6-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="369f6-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="369f6-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="369f6-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="369f6-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="369f6-268">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="369f6-268">Type of work profile password that is required.</span></span> <span data-ttu-id="369f6-269">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="369f6-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="369f6-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="369f6-270">workProfileRequirePassword</span></span>|<span data-ttu-id="369f6-271">Логический</span><span class="sxs-lookup"><span data-stu-id="369f6-271">Boolean</span></span>|<span data-ttu-id="369f6-272">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="369f6-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="369f6-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="369f6-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="369f6-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="369f6-274">Boolean</span></span>|<span data-ttu-id="369f6-275">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="369f6-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="369f6-276">Ответ</span><span class="sxs-lookup"><span data-stu-id="369f6-276">Response</span></span>
<span data-ttu-id="369f6-277">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="369f6-277">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="369f6-278">Пример</span><span class="sxs-lookup"><span data-stu-id="369f6-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="369f6-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="369f6-279">Request</span></span>
<span data-ttu-id="369f6-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="369f6-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="369f6-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="369f6-281">Response</span></span>
<span data-ttu-id="369f6-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="369f6-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






