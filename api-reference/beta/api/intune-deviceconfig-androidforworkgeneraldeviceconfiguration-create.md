---
title: Создание androidForWorkGeneralDeviceConfiguration
description: Создание нового объекта androidForWorkGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00054ecb0f5e71ebd63eb094678aa768ca06696
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933615"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="a4990-103">Создание androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4990-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a4990-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4990-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4990-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4990-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4990-106">Создание нового объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a4990-106">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4990-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4990-107">Prerequisites</span></span>
<span data-ttu-id="a4990-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4990-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4990-110">Permission type</span></span>|<span data-ttu-id="a4990-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4990-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4990-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4990-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4990-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4990-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4990-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4990-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4990-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4990-115">Not supported.</span></span>|
|<span data-ttu-id="a4990-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4990-116">Application</span></span>|<span data-ttu-id="a4990-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4990-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4990-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4990-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4990-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4990-119">Request headers</span></span>
|<span data-ttu-id="a4990-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4990-120">Header</span></span>|<span data-ttu-id="a4990-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a4990-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4990-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4990-122">Authorization</span></span>|<span data-ttu-id="a4990-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4990-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4990-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a4990-124">Accept</span></span>|<span data-ttu-id="a4990-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4990-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4990-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4990-126">Request body</span></span>
<span data-ttu-id="a4990-127">В тексте запроса добавьте представление объекта androidForWorkGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4990-127">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="a4990-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a4990-128">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="a4990-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4990-129">Property</span></span>|<span data-ttu-id="a4990-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4990-130">Type</span></span>|<span data-ttu-id="a4990-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4990-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4990-132">id</span><span class="sxs-lookup"><span data-stu-id="a4990-132">id</span></span>|<span data-ttu-id="a4990-133">String</span><span class="sxs-lookup"><span data-stu-id="a4990-133">String</span></span>|<span data-ttu-id="a4990-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4990-134">Key of the entity.</span></span> <span data-ttu-id="a4990-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4990-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a4990-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4990-137">DateTimeOffset</span></span>|<span data-ttu-id="a4990-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a4990-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a4990-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4990-140">roleScopeTagIds</span></span>|<span data-ttu-id="a4990-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a4990-141">String collection</span></span>|<span data-ttu-id="a4990-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a4990-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4990-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a4990-144">supportsScopeTags</span></span>|<span data-ttu-id="a4990-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-145">Boolean</span></span>|<span data-ttu-id="a4990-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a4990-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a4990-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a4990-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a4990-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a4990-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a4990-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4990-149">This property is read-only.</span></span> <span data-ttu-id="a4990-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4990-151">createdDateTime</span></span>|<span data-ttu-id="a4990-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4990-152">DateTimeOffset</span></span>|<span data-ttu-id="a4990-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a4990-153">DateTime the object was created.</span></span> <span data-ttu-id="a4990-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-155">description</span><span class="sxs-lookup"><span data-stu-id="a4990-155">description</span></span>|<span data-ttu-id="a4990-156">String</span><span class="sxs-lookup"><span data-stu-id="a4990-156">String</span></span>|<span data-ttu-id="a4990-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a4990-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4990-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a4990-159">displayName</span></span>|<span data-ttu-id="a4990-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a4990-160">String</span></span>|<span data-ttu-id="a4990-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a4990-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4990-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-163">version</span><span class="sxs-lookup"><span data-stu-id="a4990-163">version</span></span>|<span data-ttu-id="a4990-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-164">Int32</span></span>|<span data-ttu-id="a4990-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a4990-165">Version of the device configuration.</span></span> <span data-ttu-id="a4990-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4990-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4990-167">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a4990-167">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a4990-168">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-168">Boolean</span></span>|<span data-ttu-id="a4990-169">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="a4990-169">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a4990-170">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a4990-170">passwordBlockTrustAgents</span></span>|<span data-ttu-id="a4990-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4990-171">Boolean</span></span>|<span data-ttu-id="a4990-172">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="a4990-172">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="a4990-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a4990-173">passwordExpirationDays</span></span>|<span data-ttu-id="a4990-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-174">Int32</span></span>|<span data-ttu-id="a4990-175">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="a4990-175">Number of days before the password expires.</span></span> <span data-ttu-id="a4990-176">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a4990-176">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a4990-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a4990-177">passwordMinimumLength</span></span>|<span data-ttu-id="a4990-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-178">Int32</span></span>|<span data-ttu-id="a4990-179">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="a4990-179">Minimum length of passwords.</span></span> <span data-ttu-id="a4990-180">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a4990-180">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a4990-181">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a4990-181">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a4990-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-182">Int32</span></span>|<span data-ttu-id="a4990-183">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a4990-183">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a4990-184">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a4990-184">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a4990-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-185">Int32</span></span>|<span data-ttu-id="a4990-186">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="a4990-186">Number of previous passwords to block.</span></span> <span data-ttu-id="a4990-187">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="a4990-187">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a4990-188">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a4990-188">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a4990-189">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-189">Int32</span></span>|<span data-ttu-id="a4990-190">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="a4990-190">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="a4990-191">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="a4990-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a4990-192">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a4990-192">passwordRequiredType</span></span>|[<span data-ttu-id="a4990-193">Андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="a4990-193">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="a4990-194">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a4990-194">Type of password that is required.</span></span> <span data-ttu-id="a4990-195">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a4990-195">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a4990-196">Воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="a4990-196">workProfileDataSharingType</span></span>|[<span data-ttu-id="a4990-197">Андроидфорворккросспрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="a4990-197">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="a4990-198">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="a4990-198">Type of data sharing that is allowed.</span></span> <span data-ttu-id="a4990-199">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="a4990-199">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="a4990-200">Воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="a4990-200">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="a4990-201">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-201">Boolean</span></span>|<span data-ttu-id="a4990-202">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="a4990-202">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="a4990-203">Воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="a4990-203">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="a4990-204">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-204">Boolean</span></span>|<span data-ttu-id="a4990-205">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="a4990-205">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="a4990-206">Воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="a4990-206">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="a4990-207">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-207">Boolean</span></span>|<span data-ttu-id="a4990-208">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="a4990-208">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="a4990-209">Воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="a4990-209">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="a4990-210">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-210">Boolean</span></span>|<span data-ttu-id="a4990-211">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="a4990-211">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="a4990-212">Воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="a4990-212">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="a4990-213">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-213">Boolean</span></span>|<span data-ttu-id="a4990-214">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a4990-214">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="a4990-215">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="a4990-215">workProfileBlockCamera</span></span>|<span data-ttu-id="a4990-216">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-216">Boolean</span></span>|<span data-ttu-id="a4990-217">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-217">Block work profile camera.</span></span>|
|<span data-ttu-id="a4990-218">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="a4990-218">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="a4990-219">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-219">Boolean</span></span>|<span data-ttu-id="a4990-220">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a4990-220">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="a4990-221">Воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="a4990-221">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="a4990-222">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-222">Boolean</span></span>|<span data-ttu-id="a4990-223">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="a4990-223">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="a4990-224">Воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="a4990-224">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="a4990-225">Андроидфорворкдефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="a4990-225">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="a4990-226">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a4990-226">Type of password that is required.</span></span> <span data-ttu-id="a4990-227">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="a4990-227">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="a4990-228">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="a4990-228">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a4990-229">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-229">Boolean</span></span>|<span data-ttu-id="a4990-230">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-230">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="a4990-231">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a4990-231">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="a4990-232">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-232">Boolean</span></span>|<span data-ttu-id="a4990-233">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="a4990-233">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="a4990-234">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a4990-234">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="a4990-235">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-235">Int32</span></span>|<span data-ttu-id="a4990-236">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-236">Number of days before the work profile password expires.</span></span> <span data-ttu-id="a4990-237">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a4990-237">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a4990-238">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a4990-238">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="a4990-239">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-239">Int32</span></span>|<span data-ttu-id="a4990-240">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-240">Minimum length of work profile password.</span></span> <span data-ttu-id="a4990-241">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a4990-241">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a4990-242">Воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="a4990-242">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="a4990-243">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-243">Int32</span></span>|<span data-ttu-id="a4990-244">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-244">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="a4990-245">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a4990-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a4990-246">Воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="a4990-246">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="a4990-247">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-247">Int32</span></span>|<span data-ttu-id="a4990-248">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-248">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="a4990-249">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a4990-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a4990-250">Воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="a4990-250">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="a4990-251">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-251">Int32</span></span>|<span data-ttu-id="a4990-252">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-252">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="a4990-253">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a4990-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a4990-254">Воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="a4990-254">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="a4990-255">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-255">Int32</span></span>|<span data-ttu-id="a4990-256">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-256">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="a4990-257">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a4990-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a4990-258">Воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="a4990-258">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="a4990-259">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-259">Int32</span></span>|<span data-ttu-id="a4990-260">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-260">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="a4990-261">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a4990-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a4990-262">Воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="a4990-262">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="a4990-263">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-263">Int32</span></span>|<span data-ttu-id="a4990-264">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-264">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="a4990-265">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a4990-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a4990-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a4990-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a4990-267">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-267">Int32</span></span>|<span data-ttu-id="a4990-268">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a4990-268">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a4990-269">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a4990-269">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a4990-270">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-270">Int32</span></span>|<span data-ttu-id="a4990-271">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="a4990-271">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="a4990-272">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="a4990-272">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a4990-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a4990-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a4990-274">Int32</span><span class="sxs-lookup"><span data-stu-id="a4990-274">Int32</span></span>|<span data-ttu-id="a4990-275">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="a4990-275">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="a4990-276">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="a4990-276">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a4990-277">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a4990-277">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="a4990-278">Андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="a4990-278">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="a4990-279">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a4990-279">Type of work profile password that is required.</span></span> <span data-ttu-id="a4990-280">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a4990-280">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a4990-281">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a4990-281">workProfileRequirePassword</span></span>|<span data-ttu-id="a4990-282">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-282">Boolean</span></span>|<span data-ttu-id="a4990-283">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="a4990-283">Password is required or not for work profile</span></span>|
|<span data-ttu-id="a4990-284">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a4990-284">securityRequireVerifyApps</span></span>|<span data-ttu-id="a4990-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4990-285">Boolean</span></span>|<span data-ttu-id="a4990-286">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="a4990-286">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="a4990-287">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="a4990-287">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="a4990-288">Строка</span><span class="sxs-lookup"><span data-stu-id="a4990-288">String</span></span>|<span data-ttu-id="a4990-289">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="a4990-289">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="a4990-290">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="a4990-290">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="a4990-291">Логический</span><span class="sxs-lookup"><span data-stu-id="a4990-291">Boolean</span></span>|<span data-ttu-id="a4990-292">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="a4990-292">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="a4990-293">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4990-293">Response</span></span>
<span data-ttu-id="a4990-294">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4990-294">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4990-295">Пример</span><span class="sxs-lookup"><span data-stu-id="a4990-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4990-296">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4990-296">Request</span></span>
<span data-ttu-id="a4990-297">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4990-297">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2038

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="a4990-298">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4990-298">Response</span></span>
<span data-ttu-id="a4990-p128">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4990-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2210

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```




