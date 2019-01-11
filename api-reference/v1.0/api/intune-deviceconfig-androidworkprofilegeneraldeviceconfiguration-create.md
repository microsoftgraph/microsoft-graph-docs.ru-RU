---
title: Создание androidWorkProfileGeneralDeviceConfiguration
description: Создание нового объекта androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f50d028de9695ecda22339ef5e9da5b579188440
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851522"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="e2964-103">Создание androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2964-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e2964-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2964-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2964-105">Создание нового объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2964-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2964-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2964-106">Prerequisites</span></span>
<span data-ttu-id="e2964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2964-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2964-109">Permission type</span></span>|<span data-ttu-id="e2964-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2964-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2964-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2964-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2964-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2964-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2964-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2964-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2964-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2964-114">Not supported.</span></span>|
|<span data-ttu-id="e2964-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2964-115">Application</span></span>|<span data-ttu-id="e2964-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2964-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2964-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2964-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2964-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2964-118">Request headers</span></span>
|<span data-ttu-id="e2964-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2964-119">Header</span></span>|<span data-ttu-id="e2964-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e2964-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2964-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2964-121">Authorization</span></span>|<span data-ttu-id="e2964-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e2964-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2964-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e2964-123">Accept</span></span>|<span data-ttu-id="e2964-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e2964-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2964-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2964-125">Request body</span></span>
<span data-ttu-id="e2964-126">В тексте запроса укажите представление JSON для объекта androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2964-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e2964-127">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2964-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e2964-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2964-128">Property</span></span>|<span data-ttu-id="e2964-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e2964-129">Type</span></span>|<span data-ttu-id="e2964-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e2964-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2964-131">id</span><span class="sxs-lookup"><span data-stu-id="e2964-131">id</span></span>|<span data-ttu-id="e2964-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e2964-132">String</span></span>|<span data-ttu-id="e2964-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2964-133">Key of the entity.</span></span> <span data-ttu-id="e2964-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2964-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2964-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2964-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e2964-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2964-136">DateTimeOffset</span></span>|<span data-ttu-id="e2964-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2964-137">DateTime the object was last modified.</span></span> <span data-ttu-id="e2964-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2964-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2964-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2964-139">createdDateTime</span></span>|<span data-ttu-id="e2964-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2964-140">DateTimeOffset</span></span>|<span data-ttu-id="e2964-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2964-141">DateTime the object was created.</span></span> <span data-ttu-id="e2964-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2964-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2964-143">описание</span><span class="sxs-lookup"><span data-stu-id="e2964-143">description</span></span>|<span data-ttu-id="e2964-144">Строка</span><span class="sxs-lookup"><span data-stu-id="e2964-144">String</span></span>|<span data-ttu-id="e2964-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2964-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2964-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2964-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2964-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e2964-147">displayName</span></span>|<span data-ttu-id="e2964-148">Строка</span><span class="sxs-lookup"><span data-stu-id="e2964-148">String</span></span>|<span data-ttu-id="e2964-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2964-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2964-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2964-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2964-151">version</span><span class="sxs-lookup"><span data-stu-id="e2964-151">version</span></span>|<span data-ttu-id="e2964-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-152">Int32</span></span>|<span data-ttu-id="e2964-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2964-153">Version of the device configuration.</span></span> <span data-ttu-id="e2964-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2964-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2964-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e2964-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e2964-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2964-156">Boolean</span></span>|<span data-ttu-id="e2964-157">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="e2964-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e2964-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e2964-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e2964-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2964-159">Boolean</span></span>|<span data-ttu-id="e2964-160">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="e2964-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e2964-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e2964-161">passwordExpirationDays</span></span>|<span data-ttu-id="e2964-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-162">Int32</span></span>|<span data-ttu-id="e2964-163">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="e2964-163">Number of days before the password expires.</span></span> <span data-ttu-id="e2964-164">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="e2964-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e2964-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e2964-165">passwordMinimumLength</span></span>|<span data-ttu-id="e2964-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-166">Int32</span></span>|<span data-ttu-id="e2964-167">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="e2964-167">Minimum length of passwords.</span></span> <span data-ttu-id="e2964-168">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="e2964-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e2964-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e2964-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e2964-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-170">Int32</span></span>|<span data-ttu-id="e2964-171">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="e2964-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e2964-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e2964-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e2964-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-173">Int32</span></span>|<span data-ttu-id="e2964-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="e2964-174">Number of previous passwords to block.</span></span> <span data-ttu-id="e2964-175">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="e2964-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e2964-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e2964-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e2964-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-177">Int32</span></span>|<span data-ttu-id="e2964-178">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="e2964-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e2964-179">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="e2964-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e2964-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e2964-180">passwordRequiredType</span></span>|[<span data-ttu-id="e2964-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e2964-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e2964-182">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e2964-182">Type of password that is required.</span></span> <span data-ttu-id="e2964-183">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e2964-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e2964-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e2964-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="e2964-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e2964-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="e2964-186">Тип данных, общий доступ к, разрешен.</span><span class="sxs-lookup"><span data-stu-id="e2964-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="e2964-187">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="e2964-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="e2964-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e2964-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="e2964-189">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-189">Boolean</span></span>|<span data-ttu-id="e2964-190">Указывает, следует ли блокировать уведомления во время устройство заблокирован.</span><span class="sxs-lookup"><span data-stu-id="e2964-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="e2964-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="e2964-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="e2964-192">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-192">Boolean</span></span>|<span data-ttu-id="e2964-193">Запретить пользователям добавление или удаление учетных записей в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="e2964-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="e2964-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="e2964-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="e2964-195">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-195">Boolean</span></span>|<span data-ttu-id="e2964-196">Разрешить bluetooth устройств для доступа к корпоративной контакты.</span><span class="sxs-lookup"><span data-stu-id="e2964-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="e2964-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e2964-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="e2964-198">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-198">Boolean</span></span>|<span data-ttu-id="e2964-199">Снимок экрана блок в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="e2964-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="e2964-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="e2964-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="e2964-201">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-201">Boolean</span></span>|<span data-ttu-id="e2964-202">Блокировки отображения рабочих профилей идентификатор звонящего в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="e2964-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="e2964-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="e2964-203">workProfileBlockCamera</span></span>|<span data-ttu-id="e2964-204">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-204">Boolean</span></span>|<span data-ttu-id="e2964-205">Камера профилей рабочего блока.</span><span class="sxs-lookup"><span data-stu-id="e2964-205">Block work profile camera.</span></span>|
|<span data-ttu-id="e2964-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="e2964-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="e2964-207">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-207">Boolean</span></span>|<span data-ttu-id="e2964-208">Блок рабочих профилей доступности контактов в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="e2964-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="e2964-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e2964-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="e2964-210">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-210">Boolean</span></span>|<span data-ttu-id="e2964-211">Логическое значение, которое указывает, включен ли параметр Запретить на нескольких профилей копирование и вставка.</span><span class="sxs-lookup"><span data-stu-id="e2964-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="e2964-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="e2964-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="e2964-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e2964-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="e2964-214">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e2964-214">Type of password that is required.</span></span> <span data-ttu-id="e2964-215">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="e2964-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e2964-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e2964-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e2964-217">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-217">Boolean</span></span>|<span data-ttu-id="e2964-218">Указывает ли блокировать отпечатка разблокировки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="e2964-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="e2964-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e2964-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="e2964-220">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-220">Boolean</span></span>|<span data-ttu-id="e2964-221">Указывает, следует ли блокировать смарт-Lock и других агенты управления безопасностью для рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="e2964-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="e2964-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e2964-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="e2964-223">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-223">Int32</span></span>|<span data-ttu-id="e2964-224">Количество дней до пароля профиля рабочих срок действия.</span><span class="sxs-lookup"><span data-stu-id="e2964-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="e2964-225">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="e2964-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e2964-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e2964-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="e2964-227">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-227">Int32</span></span>|<span data-ttu-id="e2964-228">Минимальная длина пароля профиля работой.</span><span class="sxs-lookup"><span data-stu-id="e2964-228">Minimum length of work profile password.</span></span> <span data-ttu-id="e2964-229">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="e2964-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e2964-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="e2964-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="e2964-231">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-231">Int32</span></span>|<span data-ttu-id="e2964-232">Минимальное число цифр в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="e2964-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="e2964-233">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="e2964-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e2964-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e2964-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="e2964-235">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-235">Int32</span></span>|<span data-ttu-id="e2964-236">Минимальное число не буквенные символы, требуется в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="e2964-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="e2964-237">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="e2964-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e2964-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e2964-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="e2964-239">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-239">Int32</span></span>|<span data-ttu-id="e2964-240">Минимальное число буквенные символы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="e2964-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="e2964-241">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="e2964-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e2964-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e2964-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="e2964-243">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-243">Int32</span></span>|<span data-ttu-id="e2964-244">Минимальное число строчные буквы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="e2964-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="e2964-245">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="e2964-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e2964-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e2964-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="e2964-247">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-247">Int32</span></span>|<span data-ttu-id="e2964-248">Минимальное число верхнего регистра знаков, которые необходимо в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="e2964-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="e2964-249">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="e2964-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e2964-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="e2964-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="e2964-251">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-251">Int32</span></span>|<span data-ttu-id="e2964-252">Минимальное число символов, необходимых в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="e2964-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="e2964-253">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="e2964-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e2964-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e2964-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e2964-255">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-255">Int32</span></span>|<span data-ttu-id="e2964-256">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="e2964-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e2964-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e2964-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e2964-258">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-258">Int32</span></span>|<span data-ttu-id="e2964-259">Число предыдущих паролей рабочих профилей для блокировки.</span><span class="sxs-lookup"><span data-stu-id="e2964-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="e2964-260">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="e2964-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e2964-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e2964-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e2964-262">Int32</span><span class="sxs-lookup"><span data-stu-id="e2964-262">Int32</span></span>|<span data-ttu-id="e2964-263">Число входа в сбоев перед удалением рабочих профилей и удаление всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="e2964-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="e2964-264">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="e2964-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e2964-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e2964-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="e2964-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e2964-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e2964-267">Тип рабочих профилей пароль, который является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e2964-267">Type of work profile password that is required.</span></span> <span data-ttu-id="e2964-268">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e2964-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e2964-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e2964-269">workProfileRequirePassword</span></span>|<span data-ttu-id="e2964-270">Логический</span><span class="sxs-lookup"><span data-stu-id="e2964-270">Boolean</span></span>|<span data-ttu-id="e2964-271">Пароль или не для работы профиля</span><span class="sxs-lookup"><span data-stu-id="e2964-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="e2964-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e2964-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="e2964-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2964-273">Boolean</span></span>|<span data-ttu-id="e2964-274">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="e2964-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="e2964-275">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2964-275">Response</span></span>
<span data-ttu-id="e2964-276">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e2964-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2964-277">Пример</span><span class="sxs-lookup"><span data-stu-id="e2964-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2964-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2964-278">Request</span></span>
<span data-ttu-id="e2964-279">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2964-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2964-280">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2964-280">Response</span></span>
<span data-ttu-id="e2964-p126">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e2964-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



