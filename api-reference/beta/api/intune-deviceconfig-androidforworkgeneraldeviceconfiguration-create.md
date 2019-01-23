---
title: Создание androidForWorkGeneralDeviceConfiguration
description: Создание нового объекта androidForWorkGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 40e503b04c1325567dd6fbef831ae24d5a0115e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414083"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="faaaa-103">Создание androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaaa-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="faaaa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="faaaa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faaaa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faaaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faaaa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faaaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faaaa-107">Создание нового объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="faaaa-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faaaa-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="faaaa-108">Prerequisites</span></span>
<span data-ttu-id="faaaa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="faaaa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faaaa-111">Permission type</span></span>|<span data-ttu-id="faaaa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="faaaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faaaa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faaaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="faaaa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faaaa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faaaa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faaaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faaaa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faaaa-116">Not supported.</span></span>|
|<span data-ttu-id="faaaa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faaaa-117">Application</span></span>|<span data-ttu-id="faaaa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faaaa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faaaa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faaaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="faaaa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faaaa-120">Request headers</span></span>
|<span data-ttu-id="faaaa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faaaa-121">Header</span></span>|<span data-ttu-id="faaaa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="faaaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faaaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="faaaa-123">Authorization</span></span>|<span data-ttu-id="faaaa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="faaaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faaaa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="faaaa-125">Accept</span></span>|<span data-ttu-id="faaaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="faaaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faaaa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="faaaa-127">Request body</span></span>
<span data-ttu-id="faaaa-128">В тексте запроса укажите представление JSON для объекта androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="faaaa-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="faaaa-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="faaaa-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="faaaa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="faaaa-130">Property</span></span>|<span data-ttu-id="faaaa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="faaaa-131">Type</span></span>|<span data-ttu-id="faaaa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="faaaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faaaa-133">id</span><span class="sxs-lookup"><span data-stu-id="faaaa-133">id</span></span>|<span data-ttu-id="faaaa-134">String</span><span class="sxs-lookup"><span data-stu-id="faaaa-134">String</span></span>|<span data-ttu-id="faaaa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="faaaa-135">Key of the entity.</span></span> <span data-ttu-id="faaaa-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faaaa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="faaaa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faaaa-138">DateTimeOffset</span></span>|<span data-ttu-id="faaaa-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="faaaa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="faaaa-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="faaaa-141">roleScopeTagIds</span></span>|<span data-ttu-id="faaaa-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="faaaa-142">String collection</span></span>|<span data-ttu-id="faaaa-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="faaaa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="faaaa-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="faaaa-145">supportsScopeTags</span></span>|<span data-ttu-id="faaaa-146">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-146">Boolean</span></span>|<span data-ttu-id="faaaa-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="faaaa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="faaaa-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="faaaa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="faaaa-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="faaaa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="faaaa-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faaaa-150">This property is read-only.</span></span> <span data-ttu-id="faaaa-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faaaa-152">createdDateTime</span></span>|<span data-ttu-id="faaaa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faaaa-153">DateTimeOffset</span></span>|<span data-ttu-id="faaaa-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="faaaa-154">DateTime the object was created.</span></span> <span data-ttu-id="faaaa-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-156">description</span><span class="sxs-lookup"><span data-stu-id="faaaa-156">description</span></span>|<span data-ttu-id="faaaa-157">String</span><span class="sxs-lookup"><span data-stu-id="faaaa-157">String</span></span>|<span data-ttu-id="faaaa-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="faaaa-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="faaaa-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-160">displayName</span><span class="sxs-lookup"><span data-stu-id="faaaa-160">displayName</span></span>|<span data-ttu-id="faaaa-161">String</span><span class="sxs-lookup"><span data-stu-id="faaaa-161">String</span></span>|<span data-ttu-id="faaaa-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="faaaa-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="faaaa-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-164">version</span><span class="sxs-lookup"><span data-stu-id="faaaa-164">version</span></span>|<span data-ttu-id="faaaa-165">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-165">Int32</span></span>|<span data-ttu-id="faaaa-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="faaaa-166">Version of the device configuration.</span></span> <span data-ttu-id="faaaa-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faaaa-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaaa-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="faaaa-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="faaaa-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="faaaa-169">Boolean</span></span>|<span data-ttu-id="faaaa-170">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="faaaa-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="faaaa-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="faaaa-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="faaaa-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="faaaa-172">Boolean</span></span>|<span data-ttu-id="faaaa-173">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="faaaa-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="faaaa-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="faaaa-174">passwordExpirationDays</span></span>|<span data-ttu-id="faaaa-175">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-175">Int32</span></span>|<span data-ttu-id="faaaa-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="faaaa-176">Number of days before the password expires.</span></span> <span data-ttu-id="faaaa-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="faaaa-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="faaaa-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="faaaa-178">passwordMinimumLength</span></span>|<span data-ttu-id="faaaa-179">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-179">Int32</span></span>|<span data-ttu-id="faaaa-180">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="faaaa-180">Minimum length of passwords.</span></span> <span data-ttu-id="faaaa-181">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="faaaa-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="faaaa-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="faaaa-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="faaaa-183">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-183">Int32</span></span>|<span data-ttu-id="faaaa-184">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="faaaa-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="faaaa-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="faaaa-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="faaaa-186">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-186">Int32</span></span>|<span data-ttu-id="faaaa-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="faaaa-187">Number of previous passwords to block.</span></span> <span data-ttu-id="faaaa-188">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="faaaa-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="faaaa-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="faaaa-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="faaaa-190">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-190">Int32</span></span>|<span data-ttu-id="faaaa-191">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="faaaa-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="faaaa-192">Допустимые значения 1 до 16</span><span class="sxs-lookup"><span data-stu-id="faaaa-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faaaa-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="faaaa-193">passwordRequiredType</span></span>|[<span data-ttu-id="faaaa-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="faaaa-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="faaaa-195">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="faaaa-195">Type of password that is required.</span></span> <span data-ttu-id="faaaa-196">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="faaaa-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="faaaa-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="faaaa-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="faaaa-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="faaaa-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="faaaa-199">Тип данных, общий доступ к, разрешен.</span><span class="sxs-lookup"><span data-stu-id="faaaa-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="faaaa-200">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="faaaa-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="faaaa-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="faaaa-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="faaaa-202">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-202">Boolean</span></span>|<span data-ttu-id="faaaa-203">Указывает, следует ли блокировать уведомления во время устройство заблокирован.</span><span class="sxs-lookup"><span data-stu-id="faaaa-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="faaaa-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="faaaa-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="faaaa-205">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-205">Boolean</span></span>|<span data-ttu-id="faaaa-206">Запретить пользователям добавление или удаление учетных записей в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="faaaa-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="faaaa-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="faaaa-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="faaaa-208">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-208">Boolean</span></span>|<span data-ttu-id="faaaa-209">Разрешить bluetooth устройств для доступа к корпоративной контакты.</span><span class="sxs-lookup"><span data-stu-id="faaaa-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="faaaa-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="faaaa-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="faaaa-211">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-211">Boolean</span></span>|<span data-ttu-id="faaaa-212">Снимок экрана блок в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="faaaa-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="faaaa-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="faaaa-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="faaaa-214">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-214">Boolean</span></span>|<span data-ttu-id="faaaa-215">Блокировки отображения рабочих профилей идентификатор звонящего в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="faaaa-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="faaaa-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="faaaa-216">workProfileBlockCamera</span></span>|<span data-ttu-id="faaaa-217">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-217">Boolean</span></span>|<span data-ttu-id="faaaa-218">Камера профилей рабочего блока.</span><span class="sxs-lookup"><span data-stu-id="faaaa-218">Block work profile camera.</span></span>|
|<span data-ttu-id="faaaa-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="faaaa-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="faaaa-220">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-220">Boolean</span></span>|<span data-ttu-id="faaaa-221">Блок рабочих профилей доступности контактов в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="faaaa-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="faaaa-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="faaaa-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="faaaa-223">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-223">Boolean</span></span>|<span data-ttu-id="faaaa-224">Логическое значение, которое указывает, включен ли параметр Запретить на нескольких профилей копирование и вставка.</span><span class="sxs-lookup"><span data-stu-id="faaaa-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="faaaa-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="faaaa-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="faaaa-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="faaaa-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="faaaa-227">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="faaaa-227">Type of password that is required.</span></span> <span data-ttu-id="faaaa-228">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="faaaa-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="faaaa-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="faaaa-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="faaaa-230">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-230">Boolean</span></span>|<span data-ttu-id="faaaa-231">Указывает ли блокировать отпечатка разблокировки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="faaaa-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="faaaa-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="faaaa-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="faaaa-233">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-233">Boolean</span></span>|<span data-ttu-id="faaaa-234">Указывает, следует ли блокировать смарт-Lock и других агенты управления безопасностью для рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="faaaa-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="faaaa-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="faaaa-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="faaaa-236">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-236">Int32</span></span>|<span data-ttu-id="faaaa-237">Количество дней до пароля профиля рабочих срок действия.</span><span class="sxs-lookup"><span data-stu-id="faaaa-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="faaaa-238">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="faaaa-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="faaaa-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="faaaa-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="faaaa-240">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-240">Int32</span></span>|<span data-ttu-id="faaaa-241">Минимальная длина пароля профиля работой.</span><span class="sxs-lookup"><span data-stu-id="faaaa-241">Minimum length of work profile password.</span></span> <span data-ttu-id="faaaa-242">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="faaaa-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="faaaa-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="faaaa-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="faaaa-244">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-244">Int32</span></span>|<span data-ttu-id="faaaa-245">Минимальное число цифр в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="faaaa-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="faaaa-246">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="faaaa-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="faaaa-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="faaaa-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="faaaa-248">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-248">Int32</span></span>|<span data-ttu-id="faaaa-249">Минимальное число не буквенные символы, требуется в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="faaaa-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="faaaa-250">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="faaaa-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="faaaa-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="faaaa-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="faaaa-252">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-252">Int32</span></span>|<span data-ttu-id="faaaa-253">Минимальное число буквенные символы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="faaaa-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="faaaa-254">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="faaaa-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="faaaa-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="faaaa-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="faaaa-256">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-256">Int32</span></span>|<span data-ttu-id="faaaa-257">Минимальное число строчные буквы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="faaaa-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="faaaa-258">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="faaaa-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="faaaa-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="faaaa-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="faaaa-260">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-260">Int32</span></span>|<span data-ttu-id="faaaa-261">Минимальное число верхнего регистра знаков, которые необходимо в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="faaaa-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="faaaa-262">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="faaaa-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="faaaa-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="faaaa-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="faaaa-264">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-264">Int32</span></span>|<span data-ttu-id="faaaa-265">Минимальное число символов, необходимых в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="faaaa-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="faaaa-266">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="faaaa-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="faaaa-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="faaaa-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="faaaa-268">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-268">Int32</span></span>|<span data-ttu-id="faaaa-269">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="faaaa-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="faaaa-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="faaaa-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="faaaa-271">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-271">Int32</span></span>|<span data-ttu-id="faaaa-272">Число предыдущих паролей рабочих профилей для блокировки.</span><span class="sxs-lookup"><span data-stu-id="faaaa-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="faaaa-273">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="faaaa-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="faaaa-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="faaaa-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="faaaa-275">Int32</span><span class="sxs-lookup"><span data-stu-id="faaaa-275">Int32</span></span>|<span data-ttu-id="faaaa-276">Число входа в сбоев перед удалением рабочих профилей и удаление всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="faaaa-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="faaaa-277">Допустимые значения 1 до 16</span><span class="sxs-lookup"><span data-stu-id="faaaa-277">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faaaa-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="faaaa-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="faaaa-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="faaaa-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="faaaa-280">Тип рабочих профилей пароль, который является обязательным.</span><span class="sxs-lookup"><span data-stu-id="faaaa-280">Type of work profile password that is required.</span></span> <span data-ttu-id="faaaa-281">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="faaaa-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="faaaa-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="faaaa-282">workProfileRequirePassword</span></span>|<span data-ttu-id="faaaa-283">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-283">Boolean</span></span>|<span data-ttu-id="faaaa-284">Пароль или не для работы профиля</span><span class="sxs-lookup"><span data-stu-id="faaaa-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="faaaa-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="faaaa-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="faaaa-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="faaaa-286">Boolean</span></span>|<span data-ttu-id="faaaa-287">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="faaaa-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="faaaa-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="faaaa-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="faaaa-289">String</span><span class="sxs-lookup"><span data-stu-id="faaaa-289">String</span></span>|<span data-ttu-id="faaaa-290">Включите режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="faaaa-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="faaaa-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="faaaa-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="faaaa-292">Логический</span><span class="sxs-lookup"><span data-stu-id="faaaa-292">Boolean</span></span>|<span data-ttu-id="faaaa-293">Включите режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="faaaa-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="faaaa-294">Отклик</span><span class="sxs-lookup"><span data-stu-id="faaaa-294">Response</span></span>
<span data-ttu-id="faaaa-295">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="faaaa-295">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faaaa-296">Пример</span><span class="sxs-lookup"><span data-stu-id="faaaa-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="faaaa-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="faaaa-297">Request</span></span>
<span data-ttu-id="faaaa-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="faaaa-298">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="faaaa-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="faaaa-299">Response</span></span>
<span data-ttu-id="faaaa-p129">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="faaaa-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




