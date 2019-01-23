---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойства объекта androidWorkProfileGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0cec0b230b9e8735b5071920ccba8639ea58de2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410037"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="2b6f4-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b6f4-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2b6f4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b6f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b6f4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b6f4-107">Обновление свойства объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2b6f4-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b6f4-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2b6f4-108">Prerequisites</span></span>
<span data-ttu-id="2b6f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2b6f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b6f4-111">Permission type</span></span>|<span data-ttu-id="2b6f4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b6f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b6f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b6f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b6f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-116">Not supported.</span></span>|
|<span data-ttu-id="2b6f4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b6f4-117">Application</span></span>|<span data-ttu-id="2b6f4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b6f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2b6f4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b6f4-120">Request headers</span></span>
|<span data-ttu-id="2b6f4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b6f4-121">Header</span></span>|<span data-ttu-id="2b6f4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b6f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b6f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b6f4-123">Authorization</span></span>|<span data-ttu-id="2b6f4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b6f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b6f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b6f4-125">Accept</span></span>|<span data-ttu-id="2b6f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b6f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6f4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b6f4-127">Request body</span></span>
<span data-ttu-id="2b6f4-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2b6f4-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="2b6f4-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="2b6f4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b6f4-130">Property</span></span>|<span data-ttu-id="2b6f4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b6f4-131">Type</span></span>|<span data-ttu-id="2b6f4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b6f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b6f4-133">id</span><span class="sxs-lookup"><span data-stu-id="2b6f4-133">id</span></span>|<span data-ttu-id="2b6f4-134">String</span><span class="sxs-lookup"><span data-stu-id="2b6f4-134">String</span></span>|<span data-ttu-id="2b6f4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-135">Key of the entity.</span></span> <span data-ttu-id="2b6f4-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b6f4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2b6f4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6f4-138">DateTimeOffset</span></span>|<span data-ttu-id="2b6f4-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2b6f4-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b6f4-141">roleScopeTagIds</span></span>|<span data-ttu-id="2b6f4-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b6f4-142">String collection</span></span>|<span data-ttu-id="2b6f4-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b6f4-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b6f4-145">supportsScopeTags</span></span>|<span data-ttu-id="2b6f4-146">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-146">Boolean</span></span>|<span data-ttu-id="2b6f4-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b6f4-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b6f4-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b6f4-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-150">This property is read-only.</span></span> <span data-ttu-id="2b6f4-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b6f4-152">createdDateTime</span></span>|<span data-ttu-id="2b6f4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6f4-153">DateTimeOffset</span></span>|<span data-ttu-id="2b6f4-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-154">DateTime the object was created.</span></span> <span data-ttu-id="2b6f4-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-156">description</span><span class="sxs-lookup"><span data-stu-id="2b6f4-156">description</span></span>|<span data-ttu-id="2b6f4-157">String</span><span class="sxs-lookup"><span data-stu-id="2b6f4-157">String</span></span>|<span data-ttu-id="2b6f4-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b6f4-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2b6f4-160">displayName</span></span>|<span data-ttu-id="2b6f4-161">String</span><span class="sxs-lookup"><span data-stu-id="2b6f4-161">String</span></span>|<span data-ttu-id="2b6f4-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b6f4-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-164">version</span><span class="sxs-lookup"><span data-stu-id="2b6f4-164">version</span></span>|<span data-ttu-id="2b6f4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-165">Int32</span></span>|<span data-ttu-id="2b6f4-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-166">Version of the device configuration.</span></span> <span data-ttu-id="2b6f4-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b6f4-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2b6f4-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2b6f4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b6f4-169">Boolean</span></span>|<span data-ttu-id="2b6f4-170">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2b6f4-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2b6f4-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="2b6f4-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b6f4-172">Boolean</span></span>|<span data-ttu-id="2b6f4-173">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="2b6f4-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2b6f4-174">passwordExpirationDays</span></span>|<span data-ttu-id="2b6f4-175">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-175">Int32</span></span>|<span data-ttu-id="2b6f4-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-176">Number of days before the password expires.</span></span> <span data-ttu-id="2b6f4-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2b6f4-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2b6f4-178">passwordMinimumLength</span></span>|<span data-ttu-id="2b6f4-179">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-179">Int32</span></span>|<span data-ttu-id="2b6f4-180">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-180">Minimum length of passwords.</span></span> <span data-ttu-id="2b6f4-181">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2b6f4-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2b6f4-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2b6f4-183">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-183">Int32</span></span>|<span data-ttu-id="2b6f4-184">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2b6f4-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2b6f4-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2b6f4-186">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-186">Int32</span></span>|<span data-ttu-id="2b6f4-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-187">Number of previous passwords to block.</span></span> <span data-ttu-id="2b6f4-188">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="2b6f4-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2b6f4-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2b6f4-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2b6f4-190">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-190">Int32</span></span>|<span data-ttu-id="2b6f4-191">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="2b6f4-192">Допустимые значения 1 до 16</span><span class="sxs-lookup"><span data-stu-id="2b6f4-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b6f4-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-193">passwordRequiredType</span></span>|[<span data-ttu-id="2b6f4-194">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-194">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2b6f4-195">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-195">Type of password that is required.</span></span> <span data-ttu-id="2b6f4-196">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2b6f4-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="2b6f4-198">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-198">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="2b6f4-199">Тип данных, общий доступ к, разрешен.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="2b6f4-200">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="2b6f4-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="2b6f4-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="2b6f4-202">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-202">Boolean</span></span>|<span data-ttu-id="2b6f4-203">Указывает, следует ли блокировать уведомления во время устройство заблокирован.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="2b6f4-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="2b6f4-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="2b6f4-205">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-205">Boolean</span></span>|<span data-ttu-id="2b6f4-206">Запретить пользователям добавление или удаление учетных записей в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="2b6f4-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="2b6f4-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="2b6f4-208">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-208">Boolean</span></span>|<span data-ttu-id="2b6f4-209">Разрешить bluetooth устройств для доступа к корпоративной контакты.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="2b6f4-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2b6f4-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="2b6f4-211">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-211">Boolean</span></span>|<span data-ttu-id="2b6f4-212">Снимок экрана блок в профиле работой.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="2b6f4-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="2b6f4-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="2b6f4-214">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-214">Boolean</span></span>|<span data-ttu-id="2b6f4-215">Блокировки отображения рабочих профилей идентификатор звонящего в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="2b6f4-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="2b6f4-216">workProfileBlockCamera</span></span>|<span data-ttu-id="2b6f4-217">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-217">Boolean</span></span>|<span data-ttu-id="2b6f4-218">Камера профилей рабочего блока.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-218">Block work profile camera.</span></span>|
|<span data-ttu-id="2b6f4-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="2b6f4-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="2b6f4-220">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-220">Boolean</span></span>|<span data-ttu-id="2b6f4-221">Блок рабочих профилей доступности контактов в личный профиль.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="2b6f4-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="2b6f4-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="2b6f4-223">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-223">Boolean</span></span>|<span data-ttu-id="2b6f4-224">Логическое значение, которое указывает, включен ли параметр Запретить на нескольких профилей копирование и вставка.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="2b6f4-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="2b6f4-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="2b6f4-226">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-226">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="2b6f4-227">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-227">Type of password that is required.</span></span> <span data-ttu-id="2b6f4-228">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="2b6f4-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2b6f4-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2b6f4-230">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-230">Boolean</span></span>|<span data-ttu-id="2b6f4-231">Указывает ли блокировать отпечатка разблокировки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="2b6f4-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2b6f4-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="2b6f4-233">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-233">Boolean</span></span>|<span data-ttu-id="2b6f4-234">Указывает, следует ли блокировать смарт-Lock и других агенты управления безопасностью для рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="2b6f4-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2b6f4-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="2b6f4-236">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-236">Int32</span></span>|<span data-ttu-id="2b6f4-237">Количество дней до пароля профиля рабочих срок действия.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="2b6f4-238">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2b6f4-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2b6f4-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="2b6f4-240">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-240">Int32</span></span>|<span data-ttu-id="2b6f4-241">Минимальная длина пароля профиля работой.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-241">Minimum length of work profile password.</span></span> <span data-ttu-id="2b6f4-242">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2b6f4-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="2b6f4-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="2b6f4-244">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-244">Int32</span></span>|<span data-ttu-id="2b6f4-245">Минимальное число цифр в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="2b6f4-246">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b6f4-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b6f4-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2b6f4-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="2b6f4-248">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-248">Int32</span></span>|<span data-ttu-id="2b6f4-249">Минимальное число не буквенные символы, требуется в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="2b6f4-250">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b6f4-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b6f4-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2b6f4-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="2b6f4-252">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-252">Int32</span></span>|<span data-ttu-id="2b6f4-253">Минимальное число буквенные символы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="2b6f4-254">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b6f4-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b6f4-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2b6f4-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="2b6f4-256">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-256">Int32</span></span>|<span data-ttu-id="2b6f4-257">Минимальное число строчные буквы в рабочих профилей пароль требуется.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="2b6f4-258">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b6f4-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b6f4-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2b6f4-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="2b6f4-260">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-260">Int32</span></span>|<span data-ttu-id="2b6f4-261">Минимальное число верхнего регистра знаков, которые необходимо в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="2b6f4-262">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b6f4-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b6f4-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="2b6f4-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="2b6f4-264">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-264">Int32</span></span>|<span data-ttu-id="2b6f4-265">Минимальное число символов, необходимых в рабочих профилей пароль.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="2b6f4-266">Допустимые значения 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b6f4-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b6f4-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2b6f4-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2b6f4-268">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-268">Int32</span></span>|<span data-ttu-id="2b6f4-269">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="2b6f4-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2b6f4-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2b6f4-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2b6f4-271">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-271">Int32</span></span>|<span data-ttu-id="2b6f4-272">Число предыдущих паролей рабочих профилей для блокировки.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="2b6f4-273">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="2b6f4-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2b6f4-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2b6f4-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2b6f4-275">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6f4-275">Int32</span></span>|<span data-ttu-id="2b6f4-276">Число входа в сбоев перед удалением рабочих профилей и удаление всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="2b6f4-277">Допустимые значения 1 до 16</span><span class="sxs-lookup"><span data-stu-id="2b6f4-277">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b6f4-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="2b6f4-279">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2b6f4-279">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2b6f4-280">Тип рабочих профилей пароль, который является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-280">Type of work profile password that is required.</span></span> <span data-ttu-id="2b6f4-281">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2b6f4-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="2b6f4-282">workProfileRequirePassword</span></span>|<span data-ttu-id="2b6f4-283">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-283">Boolean</span></span>|<span data-ttu-id="2b6f4-284">Пароль или не для работы профиля</span><span class="sxs-lookup"><span data-stu-id="2b6f4-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="2b6f4-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2b6f4-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="2b6f4-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b6f4-286">Boolean</span></span>|<span data-ttu-id="2b6f4-287">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="2b6f4-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="2b6f4-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="2b6f4-289">String</span><span class="sxs-lookup"><span data-stu-id="2b6f4-289">String</span></span>|<span data-ttu-id="2b6f4-290">Включите режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="2b6f4-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="2b6f4-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="2b6f4-292">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6f4-292">Boolean</span></span>|<span data-ttu-id="2b6f4-293">Включите режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="2b6f4-294">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b6f4-294">Response</span></span>
<span data-ttu-id="2b6f4-295">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-295">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b6f4-296">Пример</span><span class="sxs-lookup"><span data-stu-id="2b6f4-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b6f4-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b6f4-297">Request</span></span>
<span data-ttu-id="2b6f4-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="2b6f4-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b6f4-299">Response</span></span>
<span data-ttu-id="2b6f4-p129">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b6f4-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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




