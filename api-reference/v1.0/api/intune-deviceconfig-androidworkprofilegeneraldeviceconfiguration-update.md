---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойства объекта androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 7eb65cdcfeebc4ee10edde68fa952e5555861502
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305973"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="9d91c-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d91c-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="9d91c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d91c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d91c-105">Обновление свойства объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9d91c-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d91c-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d91c-106">Prerequisites</span></span>
<span data-ttu-id="9d91c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d91c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d91c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d91c-109">Permission type</span></span>|<span data-ttu-id="9d91c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d91c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d91c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d91c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d91c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d91c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d91c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d91c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d91c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d91c-114">Not supported.</span></span>|
|<span data-ttu-id="9d91c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d91c-115">Application</span></span>|<span data-ttu-id="9d91c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d91c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d91c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d91c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9d91c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d91c-118">Request headers</span></span>
|<span data-ttu-id="9d91c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d91c-119">Header</span></span>|<span data-ttu-id="9d91c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9d91c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d91c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d91c-121">Authorization</span></span>|<span data-ttu-id="9d91c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9d91c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d91c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9d91c-123">Accept</span></span>|<span data-ttu-id="9d91c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d91c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d91c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d91c-125">Request body</span></span>
<span data-ttu-id="9d91c-126">В тексте запроса укажите представление JSON для объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9d91c-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="9d91c-127">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="9d91c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d91c-128">Property</span></span>|<span data-ttu-id="9d91c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9d91c-129">Type</span></span>|<span data-ttu-id="9d91c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9d91c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d91c-131">id</span><span class="sxs-lookup"><span data-stu-id="9d91c-131">id</span></span>|<span data-ttu-id="9d91c-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9d91c-132">String</span></span>|<span data-ttu-id="9d91c-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d91c-133">Key of the entity.</span></span> <span data-ttu-id="9d91c-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d91c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d91c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9d91c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d91c-136">DateTimeOffset</span></span>|<span data-ttu-id="9d91c-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9d91c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="9d91c-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d91c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d91c-139">createdDateTime</span></span>|<span data-ttu-id="9d91c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d91c-140">DateTimeOffset</span></span>|<span data-ttu-id="9d91c-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9d91c-141">DateTime the object was created.</span></span> <span data-ttu-id="9d91c-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d91c-143">описание</span><span class="sxs-lookup"><span data-stu-id="9d91c-143">description</span></span>|<span data-ttu-id="9d91c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="9d91c-144">String</span></span>|<span data-ttu-id="9d91c-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9d91c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d91c-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d91c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9d91c-147">displayName</span></span>|<span data-ttu-id="9d91c-148">Строка</span><span class="sxs-lookup"><span data-stu-id="9d91c-148">String</span></span>|<span data-ttu-id="9d91c-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9d91c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d91c-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d91c-151">version</span><span class="sxs-lookup"><span data-stu-id="9d91c-151">version</span></span>|<span data-ttu-id="9d91c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-152">Int32</span></span>|<span data-ttu-id="9d91c-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9d91c-153">Version of the device configuration.</span></span> <span data-ttu-id="9d91c-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d91c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d91c-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="9d91c-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="9d91c-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d91c-156">Boolean</span></span>|<span data-ttu-id="9d91c-157">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="9d91c-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="9d91c-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="9d91c-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="9d91c-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d91c-159">Boolean</span></span>|<span data-ttu-id="9d91c-160">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="9d91c-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="9d91c-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9d91c-161">passwordExpirationDays</span></span>|<span data-ttu-id="9d91c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-162">Int32</span></span>|<span data-ttu-id="9d91c-163">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="9d91c-163">Number of days before the password expires.</span></span> <span data-ttu-id="9d91c-164">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="9d91c-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9d91c-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9d91c-165">passwordMinimumLength</span></span>|<span data-ttu-id="9d91c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-166">Int32</span></span>|<span data-ttu-id="9d91c-167">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="9d91c-167">Minimum length of passwords.</span></span> <span data-ttu-id="9d91c-168">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="9d91c-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9d91c-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9d91c-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9d91c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-170">Int32</span></span>|<span data-ttu-id="9d91c-171">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="9d91c-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9d91c-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9d91c-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9d91c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-173">Int32</span></span>|<span data-ttu-id="9d91c-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="9d91c-174">Number of previous passwords to block.</span></span> <span data-ttu-id="9d91c-175">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="9d91c-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9d91c-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9d91c-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9d91c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-177">Int32</span></span>|<span data-ttu-id="9d91c-178">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="9d91c-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="9d91c-179">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="9d91c-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9d91c-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9d91c-180">passwordRequiredType</span></span>|[<span data-ttu-id="9d91c-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9d91c-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="9d91c-182">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="9d91c-182">Type of password that is required.</span></span> <span data-ttu-id="9d91c-183">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="9d91c-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="9d91c-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="9d91c-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="9d91c-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="9d91c-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="9d91c-186">Тип данных, общий доступ к, разрешен.</span><span class="sxs-lookup"><span data-stu-id="9d91c-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="9d91c-187">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="9d91c-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="9d91c-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="9d91c-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="9d91c-189">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-189">Boolean</span></span>|<span data-ttu-id="9d91c-190">Указывает, следует ли блокировать уведомления во время устройство заблокирован.</span><span class="sxs-lookup"><span data-stu-id="9d91c-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="9d91c-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="9d91c-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="9d91c-192">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-192">Boolean</span></span>|<span data-ttu-id="9d91c-193">Запретить пользователям добавление или удаление учетных записей в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="9d91c-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="9d91c-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="9d91c-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="9d91c-195">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-195">Boolean</span></span>|<span data-ttu-id="9d91c-196">Разрешить bluetooth устройств для доступа к корпоративной контакты.</span><span class="sxs-lookup"><span data-stu-id="9d91c-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="9d91c-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="9d91c-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="9d91c-198">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-198">Boolean</span></span>|<span data-ttu-id="9d91c-199">Снимок экрана блок в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="9d91c-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="9d91c-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="9d91c-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="9d91c-201">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-201">Boolean</span></span>|<span data-ttu-id="9d91c-202">Блокировки отображения рабочих профилей идентификатор звонящего в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="9d91c-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="9d91c-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="9d91c-203">workProfileBlockCamera</span></span>|<span data-ttu-id="9d91c-204">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-204">Boolean</span></span>|<span data-ttu-id="9d91c-205">Камера профилей рабочего блока.</span><span class="sxs-lookup"><span data-stu-id="9d91c-205">Block work profile camera.</span></span>|
|<span data-ttu-id="9d91c-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="9d91c-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="9d91c-207">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-207">Boolean</span></span>|<span data-ttu-id="9d91c-208">Блок рабочих профилей доступности контактов в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="9d91c-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="9d91c-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="9d91c-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="9d91c-210">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-210">Boolean</span></span>|<span data-ttu-id="9d91c-211">Логическое значение, которое указывает, включен ли параметр Запретить на нескольких профилей копирование и вставка.</span><span class="sxs-lookup"><span data-stu-id="9d91c-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="9d91c-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="9d91c-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="9d91c-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="9d91c-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="9d91c-214">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="9d91c-214">Type of password that is required.</span></span> <span data-ttu-id="9d91c-215">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="9d91c-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="9d91c-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="9d91c-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="9d91c-217">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-217">Boolean</span></span>|<span data-ttu-id="9d91c-218">Указывает ли блокировать отпечатка разблокировки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="9d91c-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="9d91c-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="9d91c-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="9d91c-220">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-220">Boolean</span></span>|<span data-ttu-id="9d91c-221">Указывает, следует ли блокировать смарт-Lock и других агенты управления безопасностью для рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="9d91c-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="9d91c-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9d91c-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="9d91c-223">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-223">Int32</span></span>|<span data-ttu-id="9d91c-224">Количество дней до пароля профиля рабочих срок действия.</span><span class="sxs-lookup"><span data-stu-id="9d91c-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="9d91c-225">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="9d91c-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9d91c-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9d91c-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="9d91c-227">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-227">Int32</span></span>|<span data-ttu-id="9d91c-228">Минимальная длина пароля профиля работой.</span><span class="sxs-lookup"><span data-stu-id="9d91c-228">Minimum length of work profile password.</span></span> <span data-ttu-id="9d91c-229">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="9d91c-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9d91c-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="9d91c-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="9d91c-231">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-231">Int32</span></span>|<span data-ttu-id="9d91c-232">Минимальное число цифр в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="9d91c-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="9d91c-233">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="9d91c-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="9d91c-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="9d91c-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="9d91c-235">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-235">Int32</span></span>|<span data-ttu-id="9d91c-236">Минимальное число не буквенные символы, требуется в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="9d91c-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="9d91c-237">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="9d91c-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="9d91c-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="9d91c-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="9d91c-239">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-239">Int32</span></span>|<span data-ttu-id="9d91c-240">Минимальное число буквенные символы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="9d91c-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="9d91c-241">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="9d91c-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="9d91c-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="9d91c-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="9d91c-243">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-243">Int32</span></span>|<span data-ttu-id="9d91c-244">Минимальное число строчные буквы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="9d91c-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="9d91c-245">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="9d91c-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="9d91c-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="9d91c-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="9d91c-247">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-247">Int32</span></span>|<span data-ttu-id="9d91c-248">Минимальное число верхнего регистра знаков, которые необходимо в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="9d91c-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="9d91c-249">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="9d91c-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="9d91c-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="9d91c-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="9d91c-251">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-251">Int32</span></span>|<span data-ttu-id="9d91c-252">Минимальное число символов, необходимых в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="9d91c-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="9d91c-253">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="9d91c-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="9d91c-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9d91c-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9d91c-255">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-255">Int32</span></span>|<span data-ttu-id="9d91c-256">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="9d91c-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9d91c-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9d91c-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9d91c-258">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-258">Int32</span></span>|<span data-ttu-id="9d91c-259">Число предыдущих паролей рабочих профилей для блокировки.</span><span class="sxs-lookup"><span data-stu-id="9d91c-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="9d91c-260">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="9d91c-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9d91c-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9d91c-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9d91c-262">Int32</span><span class="sxs-lookup"><span data-stu-id="9d91c-262">Int32</span></span>|<span data-ttu-id="9d91c-263">Число входа в сбоев перед удалением рабочих профилей и удаление всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="9d91c-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="9d91c-264">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="9d91c-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9d91c-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9d91c-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="9d91c-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9d91c-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="9d91c-267">Тип рабочих профилей пароль, который является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9d91c-267">Type of work profile password that is required.</span></span> <span data-ttu-id="9d91c-268">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="9d91c-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="9d91c-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="9d91c-269">workProfileRequirePassword</span></span>|<span data-ttu-id="9d91c-270">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9d91c-270">Boolean</span></span>|<span data-ttu-id="9d91c-271">Пароль или не для работы профиля</span><span class="sxs-lookup"><span data-stu-id="9d91c-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="9d91c-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="9d91c-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="9d91c-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d91c-273">Boolean</span></span>|<span data-ttu-id="9d91c-274">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="9d91c-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="9d91c-275">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d91c-275">Response</span></span>
<span data-ttu-id="9d91c-276">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9d91c-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d91c-277">Пример</span><span class="sxs-lookup"><span data-stu-id="9d91c-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d91c-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d91c-278">Request</span></span>
<span data-ttu-id="9d91c-279">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d91c-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d91c-280">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d91c-280">Response</span></span>
<span data-ttu-id="9d91c-p126">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9d91c-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



