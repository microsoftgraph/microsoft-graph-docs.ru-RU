---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b001e650e511a72c418704f7aac420fe25894ae9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921858"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="f649f-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="f649f-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="f649f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f649f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f649f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f649f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f649f-106">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f649f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f649f-107">Prerequisites</span></span>
<span data-ttu-id="f649f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f649f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f649f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f649f-110">Permission type</span></span>|<span data-ttu-id="f649f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f649f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f649f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f649f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f649f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f649f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f649f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f649f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f649f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f649f-115">Not supported.</span></span>|
|<span data-ttu-id="f649f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f649f-116">Application</span></span>|<span data-ttu-id="f649f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f649f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f649f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f649f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f649f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f649f-119">Request headers</span></span>
|<span data-ttu-id="f649f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f649f-120">Header</span></span>|<span data-ttu-id="f649f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f649f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f649f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f649f-122">Authorization</span></span>|<span data-ttu-id="f649f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f649f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f649f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f649f-124">Accept</span></span>|<span data-ttu-id="f649f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f649f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f649f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f649f-126">Request body</span></span>
<span data-ttu-id="f649f-127">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f649f-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="f649f-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="f649f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f649f-129">Property</span></span>|<span data-ttu-id="f649f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f649f-130">Type</span></span>|<span data-ttu-id="f649f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f649f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f649f-132">id</span><span class="sxs-lookup"><span data-stu-id="f649f-132">id</span></span>|<span data-ttu-id="f649f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f649f-133">String</span></span>|<span data-ttu-id="f649f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f649f-134">Key of the entity.</span></span> <span data-ttu-id="f649f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f649f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f649f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f649f-137">DateTimeOffset</span></span>|<span data-ttu-id="f649f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f649f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f649f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f649f-140">roleScopeTagIds</span></span>|<span data-ttu-id="f649f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f649f-141">String collection</span></span>|<span data-ttu-id="f649f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f649f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f649f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f649f-144">supportsScopeTags</span></span>|<span data-ttu-id="f649f-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f649f-145">Boolean</span></span>|<span data-ttu-id="f649f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f649f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f649f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f649f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f649f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f649f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f649f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f649f-149">This property is read-only.</span></span> <span data-ttu-id="f649f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f649f-151">createdDateTime</span></span>|<span data-ttu-id="f649f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f649f-152">DateTimeOffset</span></span>|<span data-ttu-id="f649f-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f649f-153">DateTime the object was created.</span></span> <span data-ttu-id="f649f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-155">description</span><span class="sxs-lookup"><span data-stu-id="f649f-155">description</span></span>|<span data-ttu-id="f649f-156">String</span><span class="sxs-lookup"><span data-stu-id="f649f-156">String</span></span>|<span data-ttu-id="f649f-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f649f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f649f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f649f-159">displayName</span></span>|<span data-ttu-id="f649f-160">Строка</span><span class="sxs-lookup"><span data-stu-id="f649f-160">String</span></span>|<span data-ttu-id="f649f-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f649f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f649f-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-163">version</span><span class="sxs-lookup"><span data-stu-id="f649f-163">version</span></span>|<span data-ttu-id="f649f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f649f-164">Int32</span></span>|<span data-ttu-id="f649f-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f649f-165">Version of the device configuration.</span></span> <span data-ttu-id="f649f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f649f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f649f-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f649f-167">accountManagerPolicy</span></span>|[<span data-ttu-id="f649f-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f649f-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f649f-169">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="f649f-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f649f-170">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="f649f-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f649f-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f649f-171">allowedAccounts</span></span>|[<span data-ttu-id="f649f-172">Шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="f649f-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f649f-173">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="f649f-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f649f-174">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="f649f-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="f649f-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="f649f-175">localStorage</span></span>|[<span data-ttu-id="f649f-176">Включение</span><span class="sxs-lookup"><span data-stu-id="f649f-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f649f-177">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="f649f-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="f649f-178">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f649f-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f649f-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f649f-179">allowLocalStorage</span></span>|<span data-ttu-id="f649f-180">Логический</span><span class="sxs-lookup"><span data-stu-id="f649f-180">Boolean</span></span>|<span data-ttu-id="f649f-181">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="f649f-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f649f-182">Сетаккаунтманажер</span><span class="sxs-lookup"><span data-stu-id="f649f-182">setAccountManager</span></span>|[<span data-ttu-id="f649f-183">Включение</span><span class="sxs-lookup"><span data-stu-id="f649f-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f649f-184">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="f649f-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="f649f-185">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f649f-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f649f-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f649f-186">disableAccountManager</span></span>|<span data-ttu-id="f649f-187">Логический</span><span class="sxs-lookup"><span data-stu-id="f649f-187">Boolean</span></span>|<span data-ttu-id="f649f-188">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="f649f-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f649f-189">СетедуполиЦиес</span><span class="sxs-lookup"><span data-stu-id="f649f-189">setEduPolicies</span></span>|[<span data-ttu-id="f649f-190">Включение</span><span class="sxs-lookup"><span data-stu-id="f649f-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f649f-191">Указывает, следует ли включать и отключать/не настраивать общие политики среды по умолчанию для образовательных учреждений.</span><span class="sxs-lookup"><span data-stu-id="f649f-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="f649f-192">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="f649f-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="f649f-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f649f-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f649f-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f649f-194">disableEduPolicies</span></span>|<span data-ttu-id="f649f-195">Логический</span><span class="sxs-lookup"><span data-stu-id="f649f-195">Boolean</span></span>|<span data-ttu-id="f649f-196">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="f649f-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f649f-197">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="f649f-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f649f-198">СетповерполиЦиес</span><span class="sxs-lookup"><span data-stu-id="f649f-198">setPowerPolicies</span></span>|[<span data-ttu-id="f649f-199">Включение</span><span class="sxs-lookup"><span data-stu-id="f649f-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f649f-200">Указывает, следует ли включать или отключать политики управления питанием общих ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f649f-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="f649f-201">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f649f-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f649f-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f649f-202">disablePowerPolicies</span></span>|<span data-ttu-id="f649f-203">Логический</span><span class="sxs-lookup"><span data-stu-id="f649f-203">Boolean</span></span>|<span data-ttu-id="f649f-204">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="f649f-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f649f-205">Сигнинонресуме</span><span class="sxs-lookup"><span data-stu-id="f649f-205">signInOnResume</span></span>|[<span data-ttu-id="f649f-206">Включение</span><span class="sxs-lookup"><span data-stu-id="f649f-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f649f-207">Задает требование для входа в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="f649f-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="f649f-208">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f649f-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f649f-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f649f-209">disableSignInOnResume</span></span>|<span data-ttu-id="f649f-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f649f-210">Boolean</span></span>|<span data-ttu-id="f649f-211">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="f649f-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f649f-212">enabled</span><span class="sxs-lookup"><span data-stu-id="f649f-212">enabled</span></span>|<span data-ttu-id="f649f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f649f-213">Boolean</span></span>|<span data-ttu-id="f649f-214">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="f649f-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f649f-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f649f-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f649f-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f649f-216">Int32</span></span>|<span data-ttu-id="f649f-217">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="f649f-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f649f-218">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="f649f-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f649f-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f649f-219">kioskAppDisplayName</span></span>|<span data-ttu-id="f649f-220">Строка</span><span class="sxs-lookup"><span data-stu-id="f649f-220">String</span></span>|<span data-ttu-id="f649f-221">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="f649f-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f649f-222">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="f649f-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f649f-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f649f-223">kioskAppUserModelId</span></span>|<span data-ttu-id="f649f-224">String</span><span class="sxs-lookup"><span data-stu-id="f649f-224">String</span></span>|<span data-ttu-id="f649f-225">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="f649f-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f649f-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f649f-226">maintenanceStartTime</span></span>|<span data-ttu-id="f649f-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f649f-227">TimeOfDay</span></span>|<span data-ttu-id="f649f-228">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="f649f-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="f649f-229">Фастфирстсигнин</span><span class="sxs-lookup"><span data-stu-id="f649f-229">fastFirstSignIn</span></span>|[<span data-ttu-id="f649f-230">Включение</span><span class="sxs-lookup"><span data-stu-id="f649f-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f649f-231">Указывает, следует ли автоматически подключать новые учетные записи Azure AD, не являющиеся администраторами, к предварительно настроенным локальным учетным записям кандидатов.</span><span class="sxs-lookup"><span data-stu-id="f649f-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="f649f-232">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f649f-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f649f-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="f649f-233">Response</span></span>
<span data-ttu-id="f649f-234">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f649f-234">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f649f-235">Пример</span><span class="sxs-lookup"><span data-stu-id="f649f-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="f649f-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="f649f-236">Request</span></span>
<span data-ttu-id="f649f-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f649f-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="f649f-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="f649f-238">Response</span></span>
<span data-ttu-id="f649f-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f649f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```




