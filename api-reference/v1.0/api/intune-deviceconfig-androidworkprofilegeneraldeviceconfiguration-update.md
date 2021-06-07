---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойств объекта AndroidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9e7a9e4c36823ae1b66eedaf342f6fa6574fab8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756696"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="d24ca-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d24ca-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d24ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d24ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d24ca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d24ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d24ca-106">Обновление свойств объекта [AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d24ca-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d24ca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d24ca-107">Prerequisites</span></span>
<span data-ttu-id="d24ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d24ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d24ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d24ca-110">Permission type</span></span>|<span data-ttu-id="d24ca-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d24ca-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d24ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d24ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d24ca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d24ca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d24ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d24ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d24ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d24ca-115">Not supported.</span></span>|
|<span data-ttu-id="d24ca-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d24ca-116">Application</span></span>|<span data-ttu-id="d24ca-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d24ca-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d24ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d24ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d24ca-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d24ca-119">Request headers</span></span>
|<span data-ttu-id="d24ca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d24ca-120">Header</span></span>|<span data-ttu-id="d24ca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d24ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d24ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d24ca-122">Authorization</span></span>|<span data-ttu-id="d24ca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d24ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d24ca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d24ca-124">Accept</span></span>|<span data-ttu-id="d24ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d24ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d24ca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d24ca-126">Request body</span></span>
<span data-ttu-id="d24ca-127">В теле запроса предоставляем представление JSON для [объекта AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d24ca-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="d24ca-128">В следующей таблице показаны свойства, необходимые при создании [androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d24ca-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="d24ca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d24ca-129">Property</span></span>|<span data-ttu-id="d24ca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d24ca-130">Type</span></span>|<span data-ttu-id="d24ca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d24ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d24ca-132">id</span><span class="sxs-lookup"><span data-stu-id="d24ca-132">id</span></span>|<span data-ttu-id="d24ca-133">String</span><span class="sxs-lookup"><span data-stu-id="d24ca-133">String</span></span>|<span data-ttu-id="d24ca-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d24ca-134">Key of the entity.</span></span> <span data-ttu-id="d24ca-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d24ca-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d24ca-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d24ca-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d24ca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d24ca-137">DateTimeOffset</span></span>|<span data-ttu-id="d24ca-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d24ca-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d24ca-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d24ca-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d24ca-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d24ca-140">createdDateTime</span></span>|<span data-ttu-id="d24ca-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d24ca-141">DateTimeOffset</span></span>|<span data-ttu-id="d24ca-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d24ca-142">DateTime the object was created.</span></span> <span data-ttu-id="d24ca-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d24ca-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d24ca-144">description</span><span class="sxs-lookup"><span data-stu-id="d24ca-144">description</span></span>|<span data-ttu-id="d24ca-145">String</span><span class="sxs-lookup"><span data-stu-id="d24ca-145">String</span></span>|<span data-ttu-id="d24ca-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d24ca-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d24ca-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d24ca-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d24ca-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d24ca-148">displayName</span></span>|<span data-ttu-id="d24ca-149">String</span><span class="sxs-lookup"><span data-stu-id="d24ca-149">String</span></span>|<span data-ttu-id="d24ca-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d24ca-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d24ca-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d24ca-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d24ca-152">version</span><span class="sxs-lookup"><span data-stu-id="d24ca-152">version</span></span>|<span data-ttu-id="d24ca-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-153">Int32</span></span>|<span data-ttu-id="d24ca-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d24ca-154">Version of the device configuration.</span></span> <span data-ttu-id="d24ca-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d24ca-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d24ca-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d24ca-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d24ca-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-157">Boolean</span></span>|<span data-ttu-id="d24ca-158">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="d24ca-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d24ca-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d24ca-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="d24ca-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-160">Boolean</span></span>|<span data-ttu-id="d24ca-161">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="d24ca-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="d24ca-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d24ca-162">passwordExpirationDays</span></span>|<span data-ttu-id="d24ca-163">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-163">Int32</span></span>|<span data-ttu-id="d24ca-164">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="d24ca-164">Number of days before the password expires.</span></span> <span data-ttu-id="d24ca-165">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="d24ca-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d24ca-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d24ca-166">passwordMinimumLength</span></span>|<span data-ttu-id="d24ca-167">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-167">Int32</span></span>|<span data-ttu-id="d24ca-168">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="d24ca-168">Minimum length of passwords.</span></span> <span data-ttu-id="d24ca-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="d24ca-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d24ca-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d24ca-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d24ca-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-171">Int32</span></span>|<span data-ttu-id="d24ca-172">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="d24ca-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d24ca-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d24ca-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d24ca-174">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-174">Int32</span></span>|<span data-ttu-id="d24ca-175">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="d24ca-175">Number of previous passwords to block.</span></span> <span data-ttu-id="d24ca-176">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="d24ca-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d24ca-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d24ca-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d24ca-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-178">Int32</span></span>|<span data-ttu-id="d24ca-179">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="d24ca-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="d24ca-180">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="d24ca-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="d24ca-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d24ca-181">passwordRequiredType</span></span>|[<span data-ttu-id="d24ca-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d24ca-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="d24ca-183">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="d24ca-183">Type of password that is required.</span></span> <span data-ttu-id="d24ca-184">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="d24ca-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d24ca-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d24ca-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="d24ca-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d24ca-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="d24ca-187">Тип разрешенного обмена данными.</span><span class="sxs-lookup"><span data-stu-id="d24ca-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="d24ca-188">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="d24ca-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="d24ca-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="d24ca-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="d24ca-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-190">Boolean</span></span>|<span data-ttu-id="d24ca-191">Указывает, следует ли блокировать уведомления во время блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="d24ca-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="d24ca-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="d24ca-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="d24ca-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-193">Boolean</span></span>|<span data-ttu-id="d24ca-194">Блокировать добавление и удаление учетных записей в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="d24ca-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="d24ca-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="d24ca-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-196">Boolean</span></span>|<span data-ttu-id="d24ca-197">Разрешить устройствам Bluetooth доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="d24ca-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="d24ca-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="d24ca-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="d24ca-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-199">Boolean</span></span>|<span data-ttu-id="d24ca-200">Блокировка захвата экрана в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="d24ca-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="d24ca-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="d24ca-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-202">Boolean</span></span>|<span data-ttu-id="d24ca-203">Блокировка ИД вызываемой личности вызываемой на экране работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="d24ca-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="d24ca-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="d24ca-204">workProfileBlockCamera</span></span>|<span data-ttu-id="d24ca-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-205">Boolean</span></span>|<span data-ttu-id="d24ca-206">Блокировка камеры профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-206">Block work profile camera.</span></span>|
|<span data-ttu-id="d24ca-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="d24ca-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="d24ca-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-208">Boolean</span></span>|<span data-ttu-id="d24ca-209">Блокировка доступности контактов профилей работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="d24ca-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="d24ca-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="d24ca-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="d24ca-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-211">Boolean</span></span>|<span data-ttu-id="d24ca-212">Boolean, который указывает, включен ли параметр, который не позволяет копировать/вклеить перекрестный профиль.</span><span class="sxs-lookup"><span data-stu-id="d24ca-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="d24ca-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="d24ca-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="d24ca-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="d24ca-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="d24ca-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="d24ca-215">Type of password that is required.</span></span> <span data-ttu-id="d24ca-216">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="d24ca-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="d24ca-217">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d24ca-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d24ca-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-218">Boolean</span></span>|<span data-ttu-id="d24ca-219">Указывает, следует ли блокировать разблокировку отпечатков пальцев для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="d24ca-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d24ca-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="d24ca-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-221">Boolean</span></span>|<span data-ttu-id="d24ca-222">Указывает, следует ли блокировать Smart Lock и другие агенты доверия для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="d24ca-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d24ca-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="d24ca-224">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-224">Int32</span></span>|<span data-ttu-id="d24ca-225">Количество дней до истечения срока действия пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="d24ca-226">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="d24ca-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d24ca-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d24ca-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="d24ca-228">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-228">Int32</span></span>|<span data-ttu-id="d24ca-229">Минимальная длина пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-229">Minimum length of work profile password.</span></span> <span data-ttu-id="d24ca-230">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="d24ca-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d24ca-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="d24ca-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="d24ca-232">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-232">Int32</span></span>|<span data-ttu-id="d24ca-233">Минимум # числимые символы, необходимые в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="d24ca-234">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="d24ca-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d24ca-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d24ca-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="d24ca-236">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-236">Int32</span></span>|<span data-ttu-id="d24ca-237">Минимальное количество символов без букв, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="d24ca-238">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="d24ca-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d24ca-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d24ca-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="d24ca-240">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-240">Int32</span></span>|<span data-ttu-id="d24ca-241">Минимальный # буквы символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="d24ca-242">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="d24ca-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d24ca-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d24ca-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="d24ca-244">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-244">Int32</span></span>|<span data-ttu-id="d24ca-245">Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="d24ca-246">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="d24ca-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d24ca-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d24ca-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="d24ca-248">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-248">Int32</span></span>|<span data-ttu-id="d24ca-249">Минимальный # символов верхнего уровня, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="d24ca-250">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="d24ca-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d24ca-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="d24ca-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="d24ca-252">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-252">Int32</span></span>|<span data-ttu-id="d24ca-253">Минимальный # символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="d24ca-254">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="d24ca-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d24ca-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d24ca-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d24ca-256">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-256">Int32</span></span>|<span data-ttu-id="d24ca-257">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="d24ca-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d24ca-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d24ca-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d24ca-259">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-259">Int32</span></span>|<span data-ttu-id="d24ca-260">Количество предыдущих паролей профилей работы для блокировки.</span><span class="sxs-lookup"><span data-stu-id="d24ca-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="d24ca-261">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="d24ca-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d24ca-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d24ca-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d24ca-263">Int32</span><span class="sxs-lookup"><span data-stu-id="d24ca-263">Int32</span></span>|<span data-ttu-id="d24ca-264">Количество входов в сбои, разрешенные до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="d24ca-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="d24ca-265">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="d24ca-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="d24ca-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d24ca-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="d24ca-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d24ca-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="d24ca-268">Тип необходимого пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="d24ca-268">Type of work profile password that is required.</span></span> <span data-ttu-id="d24ca-269">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="d24ca-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d24ca-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d24ca-270">workProfileRequirePassword</span></span>|<span data-ttu-id="d24ca-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-271">Boolean</span></span>|<span data-ttu-id="d24ca-272">Пароль требуется или не требуется для профиля работы</span><span class="sxs-lookup"><span data-stu-id="d24ca-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="d24ca-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="d24ca-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="d24ca-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24ca-274">Boolean</span></span>|<span data-ttu-id="d24ca-275">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="d24ca-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="d24ca-276">Ответ</span><span class="sxs-lookup"><span data-stu-id="d24ca-276">Response</span></span>
<span data-ttu-id="d24ca-277">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d24ca-277">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d24ca-278">Пример</span><span class="sxs-lookup"><span data-stu-id="d24ca-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="d24ca-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="d24ca-279">Request</span></span>
<span data-ttu-id="d24ca-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d24ca-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d24ca-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="d24ca-281">Response</span></span>
<span data-ttu-id="d24ca-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d24ca-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




