---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойств объекта androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1270136d1fa3d646dc96a60e93906c2ed37f248
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254011"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="a770f-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a770f-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a770f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a770f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a770f-105">Обновление свойств объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a770f-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a770f-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a770f-106">Prerequisites</span></span>
<span data-ttu-id="a770f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a770f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a770f-109">Permission type</span></span>|<span data-ttu-id="a770f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a770f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a770f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a770f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a770f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a770f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a770f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a770f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a770f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a770f-114">Not supported.</span></span>|
|<span data-ttu-id="a770f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a770f-115">Application</span></span>|<span data-ttu-id="a770f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a770f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a770f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a770f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a770f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a770f-118">Request headers</span></span>
|<span data-ttu-id="a770f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a770f-119">Header</span></span>|<span data-ttu-id="a770f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a770f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a770f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a770f-121">Authorization</span></span>|<span data-ttu-id="a770f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a770f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a770f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a770f-123">Accept</span></span>|<span data-ttu-id="a770f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a770f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a770f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a770f-125">Request body</span></span>
<span data-ttu-id="a770f-126">В тексте запроса добавьте представление объекта [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a770f-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a770f-127">В следующей таблице приведены свойства, необходимые при создании [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="a770f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a770f-128">Property</span></span>|<span data-ttu-id="a770f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a770f-129">Type</span></span>|<span data-ttu-id="a770f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a770f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a770f-131">id</span><span class="sxs-lookup"><span data-stu-id="a770f-131">id</span></span>|<span data-ttu-id="a770f-132">String</span><span class="sxs-lookup"><span data-stu-id="a770f-132">String</span></span>|<span data-ttu-id="a770f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a770f-133">Key of the entity.</span></span> <span data-ttu-id="a770f-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a770f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a770f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a770f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a770f-136">DateTimeOffset</span></span>|<span data-ttu-id="a770f-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a770f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a770f-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a770f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a770f-139">createdDateTime</span></span>|<span data-ttu-id="a770f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a770f-140">DateTimeOffset</span></span>|<span data-ttu-id="a770f-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a770f-141">DateTime the object was created.</span></span> <span data-ttu-id="a770f-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a770f-143">description</span><span class="sxs-lookup"><span data-stu-id="a770f-143">description</span></span>|<span data-ttu-id="a770f-144">String</span><span class="sxs-lookup"><span data-stu-id="a770f-144">String</span></span>|<span data-ttu-id="a770f-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a770f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a770f-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a770f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a770f-147">displayName</span></span>|<span data-ttu-id="a770f-148">String</span><span class="sxs-lookup"><span data-stu-id="a770f-148">String</span></span>|<span data-ttu-id="a770f-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a770f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a770f-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a770f-151">version</span><span class="sxs-lookup"><span data-stu-id="a770f-151">version</span></span>|<span data-ttu-id="a770f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-152">Int32</span></span>|<span data-ttu-id="a770f-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a770f-153">Version of the device configuration.</span></span> <span data-ttu-id="a770f-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a770f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a770f-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a770f-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a770f-156">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-156">Boolean</span></span>|<span data-ttu-id="a770f-157">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="a770f-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a770f-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a770f-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="a770f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="a770f-159">Boolean</span></span>|<span data-ttu-id="a770f-160">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="a770f-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="a770f-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a770f-161">passwordExpirationDays</span></span>|<span data-ttu-id="a770f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-162">Int32</span></span>|<span data-ttu-id="a770f-163">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="a770f-163">Number of days before the password expires.</span></span> <span data-ttu-id="a770f-164">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a770f-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a770f-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a770f-165">passwordMinimumLength</span></span>|<span data-ttu-id="a770f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-166">Int32</span></span>|<span data-ttu-id="a770f-167">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="a770f-167">Minimum length of passwords.</span></span> <span data-ttu-id="a770f-168">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a770f-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a770f-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a770f-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a770f-170">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-170">Int32</span></span>|<span data-ttu-id="a770f-171">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a770f-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a770f-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a770f-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a770f-173">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-173">Int32</span></span>|<span data-ttu-id="a770f-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="a770f-174">Number of previous passwords to block.</span></span> <span data-ttu-id="a770f-175">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="a770f-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a770f-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a770f-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a770f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-177">Int32</span></span>|<span data-ttu-id="a770f-178">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="a770f-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="a770f-179">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="a770f-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a770f-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a770f-180">passwordRequiredType</span></span>|[<span data-ttu-id="a770f-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a770f-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a770f-182">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a770f-182">Type of password that is required.</span></span> <span data-ttu-id="a770f-183">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a770f-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a770f-184">Воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="a770f-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="a770f-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a770f-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="a770f-186">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="a770f-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="a770f-187">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="a770f-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="a770f-188">Воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="a770f-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="a770f-189">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-189">Boolean</span></span>|<span data-ttu-id="a770f-190">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="a770f-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="a770f-191">Воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="a770f-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="a770f-192">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-192">Boolean</span></span>|<span data-ttu-id="a770f-193">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="a770f-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="a770f-194">Воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="a770f-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="a770f-195">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-195">Boolean</span></span>|<span data-ttu-id="a770f-196">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="a770f-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="a770f-197">Воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="a770f-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="a770f-198">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-198">Boolean</span></span>|<span data-ttu-id="a770f-199">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="a770f-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="a770f-200">Воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="a770f-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="a770f-201">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-201">Boolean</span></span>|<span data-ttu-id="a770f-202">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a770f-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="a770f-203">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="a770f-203">workProfileBlockCamera</span></span>|<span data-ttu-id="a770f-204">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-204">Boolean</span></span>|<span data-ttu-id="a770f-205">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-205">Block work profile camera.</span></span>|
|<span data-ttu-id="a770f-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="a770f-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="a770f-207">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-207">Boolean</span></span>|<span data-ttu-id="a770f-208">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a770f-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="a770f-209">Воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="a770f-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="a770f-210">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-210">Boolean</span></span>|<span data-ttu-id="a770f-211">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="a770f-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="a770f-212">Воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="a770f-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="a770f-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a770f-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="a770f-214">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a770f-214">Type of password that is required.</span></span> <span data-ttu-id="a770f-215">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="a770f-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="a770f-216">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="a770f-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a770f-217">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-217">Boolean</span></span>|<span data-ttu-id="a770f-218">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="a770f-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a770f-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="a770f-220">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-220">Boolean</span></span>|<span data-ttu-id="a770f-221">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="a770f-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="a770f-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a770f-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="a770f-223">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-223">Int32</span></span>|<span data-ttu-id="a770f-224">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="a770f-225">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a770f-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a770f-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a770f-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="a770f-227">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-227">Int32</span></span>|<span data-ttu-id="a770f-228">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-228">Minimum length of work profile password.</span></span> <span data-ttu-id="a770f-229">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a770f-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a770f-230">Воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="a770f-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="a770f-231">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-231">Int32</span></span>|<span data-ttu-id="a770f-232">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="a770f-233">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a770f-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a770f-234">Воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="a770f-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="a770f-235">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-235">Int32</span></span>|<span data-ttu-id="a770f-236">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="a770f-237">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a770f-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a770f-238">Воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="a770f-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="a770f-239">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-239">Int32</span></span>|<span data-ttu-id="a770f-240">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="a770f-241">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a770f-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a770f-242">Воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="a770f-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="a770f-243">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-243">Int32</span></span>|<span data-ttu-id="a770f-244">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="a770f-245">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a770f-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a770f-246">Воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="a770f-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="a770f-247">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-247">Int32</span></span>|<span data-ttu-id="a770f-248">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="a770f-249">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a770f-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a770f-250">Воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="a770f-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="a770f-251">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-251">Int32</span></span>|<span data-ttu-id="a770f-252">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="a770f-253">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a770f-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a770f-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a770f-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a770f-255">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-255">Int32</span></span>|<span data-ttu-id="a770f-256">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a770f-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a770f-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a770f-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a770f-258">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-258">Int32</span></span>|<span data-ttu-id="a770f-259">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="a770f-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="a770f-260">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="a770f-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a770f-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a770f-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a770f-262">Int32</span><span class="sxs-lookup"><span data-stu-id="a770f-262">Int32</span></span>|<span data-ttu-id="a770f-263">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="a770f-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="a770f-264">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="a770f-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a770f-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a770f-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="a770f-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a770f-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a770f-267">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a770f-267">Type of work profile password that is required.</span></span> <span data-ttu-id="a770f-268">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a770f-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a770f-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a770f-269">workProfileRequirePassword</span></span>|<span data-ttu-id="a770f-270">Логический</span><span class="sxs-lookup"><span data-stu-id="a770f-270">Boolean</span></span>|<span data-ttu-id="a770f-271">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="a770f-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="a770f-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a770f-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="a770f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="a770f-273">Boolean</span></span>|<span data-ttu-id="a770f-274">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="a770f-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="a770f-275">Ответ</span><span class="sxs-lookup"><span data-stu-id="a770f-275">Response</span></span>
<span data-ttu-id="a770f-276">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a770f-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a770f-277">Пример</span><span class="sxs-lookup"><span data-stu-id="a770f-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="a770f-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="a770f-278">Request</span></span>
<span data-ttu-id="a770f-279">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a770f-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a770f-280">Ответ</span><span class="sxs-lookup"><span data-stu-id="a770f-280">Response</span></span>
<span data-ttu-id="a770f-p126">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a770f-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



