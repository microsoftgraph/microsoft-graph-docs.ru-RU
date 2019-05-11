---
title: Create sharedPCConfiguration
description: Создание объекта sharedPCConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f30345bbf10bd0d0272dc4b87999951678e42db
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922117"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="bdaec-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdaec-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="bdaec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdaec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdaec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdaec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdaec-106">Создание объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdaec-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bdaec-107">Prerequisites</span></span>
<span data-ttu-id="bdaec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdaec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdaec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdaec-110">Permission type</span></span>|<span data-ttu-id="bdaec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdaec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdaec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdaec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdaec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdaec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdaec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdaec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdaec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdaec-115">Not supported.</span></span>|
|<span data-ttu-id="bdaec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdaec-116">Application</span></span>|<span data-ttu-id="bdaec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdaec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdaec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdaec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bdaec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdaec-119">Request headers</span></span>
|<span data-ttu-id="bdaec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdaec-120">Header</span></span>|<span data-ttu-id="bdaec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bdaec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdaec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdaec-122">Authorization</span></span>|<span data-ttu-id="bdaec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdaec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdaec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bdaec-124">Accept</span></span>|<span data-ttu-id="bdaec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdaec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdaec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdaec-126">Request body</span></span>
<span data-ttu-id="bdaec-127">В тексте запроса добавьте представление объекта sharedPCConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdaec-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="bdaec-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bdaec-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="bdaec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdaec-129">Property</span></span>|<span data-ttu-id="bdaec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bdaec-130">Type</span></span>|<span data-ttu-id="bdaec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bdaec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdaec-132">id</span><span class="sxs-lookup"><span data-stu-id="bdaec-132">id</span></span>|<span data-ttu-id="bdaec-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bdaec-133">String</span></span>|<span data-ttu-id="bdaec-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bdaec-134">Key of the entity.</span></span> <span data-ttu-id="bdaec-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdaec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bdaec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdaec-137">DateTimeOffset</span></span>|<span data-ttu-id="bdaec-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bdaec-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bdaec-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bdaec-140">roleScopeTagIds</span></span>|<span data-ttu-id="bdaec-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bdaec-141">String collection</span></span>|<span data-ttu-id="bdaec-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bdaec-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bdaec-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bdaec-144">supportsScopeTags</span></span>|<span data-ttu-id="bdaec-145">Логический</span><span class="sxs-lookup"><span data-stu-id="bdaec-145">Boolean</span></span>|<span data-ttu-id="bdaec-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bdaec-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bdaec-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bdaec-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bdaec-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bdaec-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bdaec-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdaec-149">This property is read-only.</span></span> <span data-ttu-id="bdaec-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdaec-151">createdDateTime</span></span>|<span data-ttu-id="bdaec-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdaec-152">DateTimeOffset</span></span>|<span data-ttu-id="bdaec-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bdaec-153">DateTime the object was created.</span></span> <span data-ttu-id="bdaec-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-155">description</span><span class="sxs-lookup"><span data-stu-id="bdaec-155">description</span></span>|<span data-ttu-id="bdaec-156">String</span><span class="sxs-lookup"><span data-stu-id="bdaec-156">String</span></span>|<span data-ttu-id="bdaec-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdaec-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bdaec-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bdaec-159">displayName</span></span>|<span data-ttu-id="bdaec-160">Строка</span><span class="sxs-lookup"><span data-stu-id="bdaec-160">String</span></span>|<span data-ttu-id="bdaec-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdaec-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bdaec-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-163">version</span><span class="sxs-lookup"><span data-stu-id="bdaec-163">version</span></span>|<span data-ttu-id="bdaec-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bdaec-164">Int32</span></span>|<span data-ttu-id="bdaec-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdaec-165">Version of the device configuration.</span></span> <span data-ttu-id="bdaec-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdaec-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdaec-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="bdaec-167">accountManagerPolicy</span></span>|[<span data-ttu-id="bdaec-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="bdaec-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="bdaec-169">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="bdaec-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="bdaec-170">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="bdaec-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="bdaec-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="bdaec-171">allowedAccounts</span></span>|[<span data-ttu-id="bdaec-172">Шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="bdaec-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="bdaec-173">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="bdaec-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="bdaec-174">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="bdaec-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="bdaec-175">localStorage</span></span>|[<span data-ttu-id="bdaec-176">Включение</span><span class="sxs-lookup"><span data-stu-id="bdaec-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bdaec-177">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="bdaec-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="bdaec-178">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bdaec-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="bdaec-179">allowLocalStorage</span></span>|<span data-ttu-id="bdaec-180">Логический</span><span class="sxs-lookup"><span data-stu-id="bdaec-180">Boolean</span></span>|<span data-ttu-id="bdaec-181">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="bdaec-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="bdaec-182">Сетаккаунтманажер</span><span class="sxs-lookup"><span data-stu-id="bdaec-182">setAccountManager</span></span>|[<span data-ttu-id="bdaec-183">Включение</span><span class="sxs-lookup"><span data-stu-id="bdaec-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bdaec-184">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="bdaec-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="bdaec-185">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bdaec-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="bdaec-186">disableAccountManager</span></span>|<span data-ttu-id="bdaec-187">Логический</span><span class="sxs-lookup"><span data-stu-id="bdaec-187">Boolean</span></span>|<span data-ttu-id="bdaec-188">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="bdaec-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="bdaec-189">СетедуполиЦиес</span><span class="sxs-lookup"><span data-stu-id="bdaec-189">setEduPolicies</span></span>|[<span data-ttu-id="bdaec-190">Включение</span><span class="sxs-lookup"><span data-stu-id="bdaec-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bdaec-191">Указывает, следует ли включать и отключать/не настраивать общие политики среды по умолчанию для образовательных учреждений.</span><span class="sxs-lookup"><span data-stu-id="bdaec-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="bdaec-192">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="bdaec-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="bdaec-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bdaec-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="bdaec-194">disableEduPolicies</span></span>|<span data-ttu-id="bdaec-195">Логический</span><span class="sxs-lookup"><span data-stu-id="bdaec-195">Boolean</span></span>|<span data-ttu-id="bdaec-196">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="bdaec-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="bdaec-197">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="bdaec-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="bdaec-198">СетповерполиЦиес</span><span class="sxs-lookup"><span data-stu-id="bdaec-198">setPowerPolicies</span></span>|[<span data-ttu-id="bdaec-199">Включение</span><span class="sxs-lookup"><span data-stu-id="bdaec-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bdaec-200">Указывает, следует ли включать или отключать политики управления питанием общих ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bdaec-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="bdaec-201">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bdaec-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="bdaec-202">disablePowerPolicies</span></span>|<span data-ttu-id="bdaec-203">Логический</span><span class="sxs-lookup"><span data-stu-id="bdaec-203">Boolean</span></span>|<span data-ttu-id="bdaec-204">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="bdaec-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="bdaec-205">Сигнинонресуме</span><span class="sxs-lookup"><span data-stu-id="bdaec-205">signInOnResume</span></span>|[<span data-ttu-id="bdaec-206">Включение</span><span class="sxs-lookup"><span data-stu-id="bdaec-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bdaec-207">Задает требование для входа в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="bdaec-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="bdaec-208">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bdaec-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="bdaec-209">disableSignInOnResume</span></span>|<span data-ttu-id="bdaec-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdaec-210">Boolean</span></span>|<span data-ttu-id="bdaec-211">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="bdaec-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="bdaec-212">enabled</span><span class="sxs-lookup"><span data-stu-id="bdaec-212">enabled</span></span>|<span data-ttu-id="bdaec-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdaec-213">Boolean</span></span>|<span data-ttu-id="bdaec-214">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="bdaec-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="bdaec-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="bdaec-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="bdaec-216">Int32</span><span class="sxs-lookup"><span data-stu-id="bdaec-216">Int32</span></span>|<span data-ttu-id="bdaec-217">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="bdaec-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="bdaec-218">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="bdaec-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="bdaec-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdaec-219">kioskAppDisplayName</span></span>|<span data-ttu-id="bdaec-220">Строка</span><span class="sxs-lookup"><span data-stu-id="bdaec-220">String</span></span>|<span data-ttu-id="bdaec-221">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="bdaec-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="bdaec-222">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="bdaec-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="bdaec-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="bdaec-223">kioskAppUserModelId</span></span>|<span data-ttu-id="bdaec-224">String</span><span class="sxs-lookup"><span data-stu-id="bdaec-224">String</span></span>|<span data-ttu-id="bdaec-225">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="bdaec-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="bdaec-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="bdaec-226">maintenanceStartTime</span></span>|<span data-ttu-id="bdaec-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bdaec-227">TimeOfDay</span></span>|<span data-ttu-id="bdaec-228">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="bdaec-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="bdaec-229">Фастфирстсигнин</span><span class="sxs-lookup"><span data-stu-id="bdaec-229">fastFirstSignIn</span></span>|[<span data-ttu-id="bdaec-230">Включение</span><span class="sxs-lookup"><span data-stu-id="bdaec-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bdaec-231">Указывает, следует ли автоматически подключать новые учетные записи Azure AD, не являющиеся администраторами, к предварительно настроенным локальным учетным записям кандидатов.</span><span class="sxs-lookup"><span data-stu-id="bdaec-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="bdaec-232">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bdaec-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="bdaec-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdaec-233">Response</span></span>
<span data-ttu-id="bdaec-234">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bdaec-234">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdaec-235">Пример</span><span class="sxs-lookup"><span data-stu-id="bdaec-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdaec-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdaec-236">Request</span></span>
<span data-ttu-id="bdaec-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdaec-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="bdaec-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdaec-238">Response</span></span>
<span data-ttu-id="bdaec-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdaec-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




