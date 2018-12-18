---
title: Создание androidForWorkGeneralDeviceConfiguration
description: Создание нового объекта androidForWorkGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: f87cf28580cbdb69de2dfb7208efe0bf38e22d0d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321639"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="359bc-103">Создание androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="359bc-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="359bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="359bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="359bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="359bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="359bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="359bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="359bc-107">Создание нового объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="359bc-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="359bc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="359bc-108">Prerequisites</span></span>
<span data-ttu-id="359bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="359bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="359bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="359bc-111">Permission type</span></span>|<span data-ttu-id="359bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="359bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="359bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="359bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="359bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="359bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="359bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="359bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="359bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="359bc-116">Not supported.</span></span>|
|<span data-ttu-id="359bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="359bc-117">Application</span></span>|<span data-ttu-id="359bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="359bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="359bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="359bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="359bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="359bc-120">Request headers</span></span>
|<span data-ttu-id="359bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="359bc-121">Header</span></span>|<span data-ttu-id="359bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="359bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="359bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="359bc-123">Authorization</span></span>|<span data-ttu-id="359bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="359bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="359bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="359bc-125">Accept</span></span>|<span data-ttu-id="359bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="359bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="359bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="359bc-127">Request body</span></span>
<span data-ttu-id="359bc-128">В тексте запроса укажите представление JSON для объекта androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="359bc-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="359bc-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="359bc-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="359bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="359bc-130">Property</span></span>|<span data-ttu-id="359bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="359bc-131">Type</span></span>|<span data-ttu-id="359bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="359bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="359bc-133">id</span><span class="sxs-lookup"><span data-stu-id="359bc-133">id</span></span>|<span data-ttu-id="359bc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="359bc-134">String</span></span>|<span data-ttu-id="359bc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="359bc-135">Key of the entity.</span></span> <span data-ttu-id="359bc-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="359bc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="359bc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="359bc-138">DateTimeOffset</span></span>|<span data-ttu-id="359bc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="359bc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="359bc-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="359bc-141">roleScopeTagIds</span></span>|<span data-ttu-id="359bc-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="359bc-142">String collection</span></span>|<span data-ttu-id="359bc-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="359bc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="359bc-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="359bc-145">supportsScopeTags</span></span>|<span data-ttu-id="359bc-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-146">Boolean</span></span>|<span data-ttu-id="359bc-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="359bc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="359bc-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="359bc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="359bc-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="359bc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="359bc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="359bc-150">This property is read-only.</span></span> <span data-ttu-id="359bc-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="359bc-152">createdDateTime</span></span>|<span data-ttu-id="359bc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="359bc-153">DateTimeOffset</span></span>|<span data-ttu-id="359bc-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="359bc-154">DateTime the object was created.</span></span> <span data-ttu-id="359bc-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-156">описание</span><span class="sxs-lookup"><span data-stu-id="359bc-156">description</span></span>|<span data-ttu-id="359bc-157">Строка</span><span class="sxs-lookup"><span data-stu-id="359bc-157">String</span></span>|<span data-ttu-id="359bc-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="359bc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="359bc-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="359bc-160">displayName</span></span>|<span data-ttu-id="359bc-161">Строка</span><span class="sxs-lookup"><span data-stu-id="359bc-161">String</span></span>|<span data-ttu-id="359bc-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="359bc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="359bc-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-164">version</span><span class="sxs-lookup"><span data-stu-id="359bc-164">version</span></span>|<span data-ttu-id="359bc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-165">Int32</span></span>|<span data-ttu-id="359bc-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="359bc-166">Version of the device configuration.</span></span> <span data-ttu-id="359bc-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="359bc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="359bc-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="359bc-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="359bc-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="359bc-169">Boolean</span></span>|<span data-ttu-id="359bc-170">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="359bc-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="359bc-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="359bc-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="359bc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="359bc-172">Boolean</span></span>|<span data-ttu-id="359bc-173">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="359bc-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="359bc-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="359bc-174">passwordExpirationDays</span></span>|<span data-ttu-id="359bc-175">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-175">Int32</span></span>|<span data-ttu-id="359bc-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="359bc-176">Number of days before the password expires.</span></span> <span data-ttu-id="359bc-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="359bc-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="359bc-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="359bc-178">passwordMinimumLength</span></span>|<span data-ttu-id="359bc-179">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-179">Int32</span></span>|<span data-ttu-id="359bc-180">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="359bc-180">Minimum length of passwords.</span></span> <span data-ttu-id="359bc-181">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="359bc-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="359bc-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="359bc-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="359bc-183">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-183">Int32</span></span>|<span data-ttu-id="359bc-184">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="359bc-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="359bc-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="359bc-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="359bc-186">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-186">Int32</span></span>|<span data-ttu-id="359bc-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="359bc-187">Number of previous passwords to block.</span></span> <span data-ttu-id="359bc-188">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="359bc-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="359bc-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="359bc-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="359bc-190">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-190">Int32</span></span>|<span data-ttu-id="359bc-191">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="359bc-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="359bc-192">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="359bc-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="359bc-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="359bc-193">passwordRequiredType</span></span>|[<span data-ttu-id="359bc-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="359bc-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="359bc-195">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="359bc-195">Type of password that is required.</span></span> <span data-ttu-id="359bc-196">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="359bc-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="359bc-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="359bc-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="359bc-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="359bc-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="359bc-199">Тип данных, общий доступ к, разрешен.</span><span class="sxs-lookup"><span data-stu-id="359bc-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="359bc-200">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="359bc-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="359bc-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="359bc-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="359bc-202">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-202">Boolean</span></span>|<span data-ttu-id="359bc-203">Указывает, следует ли блокировать уведомления во время устройство заблокирован.</span><span class="sxs-lookup"><span data-stu-id="359bc-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="359bc-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="359bc-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="359bc-205">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-205">Boolean</span></span>|<span data-ttu-id="359bc-206">Запретить пользователям добавление или удаление учетных записей в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="359bc-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="359bc-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="359bc-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="359bc-208">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-208">Boolean</span></span>|<span data-ttu-id="359bc-209">Разрешить bluetooth устройств для доступа к корпоративной контакты.</span><span class="sxs-lookup"><span data-stu-id="359bc-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="359bc-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="359bc-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="359bc-211">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-211">Boolean</span></span>|<span data-ttu-id="359bc-212">Снимок экрана блок в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="359bc-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="359bc-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="359bc-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="359bc-214">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-214">Boolean</span></span>|<span data-ttu-id="359bc-215">Блокировки отображения рабочих профилей идентификатор звонящего в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="359bc-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="359bc-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="359bc-216">workProfileBlockCamera</span></span>|<span data-ttu-id="359bc-217">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-217">Boolean</span></span>|<span data-ttu-id="359bc-218">Камера профилей рабочего блока.</span><span class="sxs-lookup"><span data-stu-id="359bc-218">Block work profile camera.</span></span>|
|<span data-ttu-id="359bc-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="359bc-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="359bc-220">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-220">Boolean</span></span>|<span data-ttu-id="359bc-221">Блок рабочих профилей доступности контактов в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="359bc-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="359bc-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="359bc-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="359bc-223">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-223">Boolean</span></span>|<span data-ttu-id="359bc-224">Логическое значение, которое указывает, включен ли параметр Запретить на нескольких профилей копирование и вставка.</span><span class="sxs-lookup"><span data-stu-id="359bc-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="359bc-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="359bc-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="359bc-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="359bc-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="359bc-227">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="359bc-227">Type of password that is required.</span></span> <span data-ttu-id="359bc-228">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="359bc-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="359bc-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="359bc-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="359bc-230">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-230">Boolean</span></span>|<span data-ttu-id="359bc-231">Указывает ли блокировать отпечатка разблокировки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="359bc-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="359bc-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="359bc-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="359bc-233">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-233">Boolean</span></span>|<span data-ttu-id="359bc-234">Указывает, следует ли блокировать смарт-Lock и других агенты управления безопасностью для рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="359bc-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="359bc-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="359bc-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="359bc-236">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-236">Int32</span></span>|<span data-ttu-id="359bc-237">Количество дней до пароля профиля рабочих срок действия.</span><span class="sxs-lookup"><span data-stu-id="359bc-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="359bc-238">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="359bc-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="359bc-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="359bc-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="359bc-240">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-240">Int32</span></span>|<span data-ttu-id="359bc-241">Минимальная длина пароля профиля работой.</span><span class="sxs-lookup"><span data-stu-id="359bc-241">Minimum length of work profile password.</span></span> <span data-ttu-id="359bc-242">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="359bc-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="359bc-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="359bc-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="359bc-244">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-244">Int32</span></span>|<span data-ttu-id="359bc-245">Минимальное число цифр в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="359bc-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="359bc-246">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="359bc-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="359bc-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="359bc-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="359bc-248">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-248">Int32</span></span>|<span data-ttu-id="359bc-249">Минимальное число не буквенные символы, требуется в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="359bc-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="359bc-250">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="359bc-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="359bc-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="359bc-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="359bc-252">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-252">Int32</span></span>|<span data-ttu-id="359bc-253">Минимальное число буквенные символы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="359bc-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="359bc-254">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="359bc-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="359bc-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="359bc-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="359bc-256">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-256">Int32</span></span>|<span data-ttu-id="359bc-257">Минимальное число строчные буквы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="359bc-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="359bc-258">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="359bc-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="359bc-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="359bc-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="359bc-260">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-260">Int32</span></span>|<span data-ttu-id="359bc-261">Минимальное число верхнего регистра знаков, которые необходимо в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="359bc-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="359bc-262">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="359bc-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="359bc-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="359bc-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="359bc-264">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-264">Int32</span></span>|<span data-ttu-id="359bc-265">Минимальное число символов, необходимых в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="359bc-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="359bc-266">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="359bc-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="359bc-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="359bc-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="359bc-268">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-268">Int32</span></span>|<span data-ttu-id="359bc-269">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="359bc-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="359bc-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="359bc-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="359bc-271">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-271">Int32</span></span>|<span data-ttu-id="359bc-272">Число предыдущих паролей рабочих профилей для блокировки.</span><span class="sxs-lookup"><span data-stu-id="359bc-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="359bc-273">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="359bc-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="359bc-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="359bc-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="359bc-275">Int32</span><span class="sxs-lookup"><span data-stu-id="359bc-275">Int32</span></span>|<span data-ttu-id="359bc-276">Число входа в сбоев перед удалением рабочих профилей и удаление всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="359bc-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="359bc-277">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="359bc-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="359bc-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="359bc-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="359bc-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="359bc-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="359bc-280">Тип рабочих профилей пароль, который является обязательным.</span><span class="sxs-lookup"><span data-stu-id="359bc-280">Type of work profile password that is required.</span></span> <span data-ttu-id="359bc-281">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="359bc-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="359bc-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="359bc-282">workProfileRequirePassword</span></span>|<span data-ttu-id="359bc-283">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-283">Boolean</span></span>|<span data-ttu-id="359bc-284">Пароль или не для работы профиля</span><span class="sxs-lookup"><span data-stu-id="359bc-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="359bc-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="359bc-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="359bc-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="359bc-286">Boolean</span></span>|<span data-ttu-id="359bc-287">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="359bc-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="359bc-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="359bc-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="359bc-289">String.</span><span class="sxs-lookup"><span data-stu-id="359bc-289">String</span></span>|<span data-ttu-id="359bc-290">Включите режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="359bc-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="359bc-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="359bc-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="359bc-292">Boolean.</span><span class="sxs-lookup"><span data-stu-id="359bc-292">Boolean</span></span>|<span data-ttu-id="359bc-293">Включите режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="359bc-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="359bc-294">Ответ</span><span class="sxs-lookup"><span data-stu-id="359bc-294">Response</span></span>
<span data-ttu-id="359bc-295">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="359bc-295">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="359bc-296">Пример</span><span class="sxs-lookup"><span data-stu-id="359bc-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="359bc-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="359bc-297">Request</span></span>
<span data-ttu-id="359bc-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="359bc-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2102

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="359bc-299">Ответ</span><span class="sxs-lookup"><span data-stu-id="359bc-299">Response</span></span>
<span data-ttu-id="359bc-p129">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="359bc-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





