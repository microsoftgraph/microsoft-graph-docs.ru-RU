---
title: Create sharedPCConfiguration
description: Создание объекта sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b28cfc822d7ced8ba0e418825ea7ad37949f18
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165109"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="534d7-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="534d7-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="534d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="534d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="534d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="534d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="534d7-106">Создание объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="534d7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="534d7-107">Prerequisites</span></span>
<span data-ttu-id="534d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="534d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="534d7-110">Permission type</span></span>|<span data-ttu-id="534d7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="534d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="534d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="534d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="534d7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="534d7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="534d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="534d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="534d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="534d7-115">Not supported.</span></span>|
|<span data-ttu-id="534d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="534d7-116">Application</span></span>|<span data-ttu-id="534d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="534d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="534d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="534d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="534d7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="534d7-119">Request headers</span></span>
|<span data-ttu-id="534d7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="534d7-120">Header</span></span>|<span data-ttu-id="534d7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="534d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="534d7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="534d7-122">Authorization</span></span>|<span data-ttu-id="534d7-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="534d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="534d7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="534d7-124">Accept</span></span>|<span data-ttu-id="534d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="534d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="534d7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="534d7-126">Request body</span></span>
<span data-ttu-id="534d7-127">В тексте запроса добавьте представление объекта sharedPCConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="534d7-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="534d7-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="534d7-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="534d7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="534d7-129">Property</span></span>|<span data-ttu-id="534d7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="534d7-130">Type</span></span>|<span data-ttu-id="534d7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="534d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="534d7-132">id</span><span class="sxs-lookup"><span data-stu-id="534d7-132">id</span></span>|<span data-ttu-id="534d7-133">String</span><span class="sxs-lookup"><span data-stu-id="534d7-133">String</span></span>|<span data-ttu-id="534d7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="534d7-134">Key of the entity.</span></span> <span data-ttu-id="534d7-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="534d7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="534d7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="534d7-137">DateTimeOffset</span></span>|<span data-ttu-id="534d7-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="534d7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="534d7-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="534d7-140">roleScopeTagIds</span></span>|<span data-ttu-id="534d7-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="534d7-141">String collection</span></span>|<span data-ttu-id="534d7-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="534d7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="534d7-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="534d7-144">supportsScopeTags</span></span>|<span data-ttu-id="534d7-145">Логический</span><span class="sxs-lookup"><span data-stu-id="534d7-145">Boolean</span></span>|<span data-ttu-id="534d7-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="534d7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="534d7-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="534d7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="534d7-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="534d7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="534d7-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="534d7-149">This property is read-only.</span></span> <span data-ttu-id="534d7-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="534d7-151">createdDateTime</span></span>|<span data-ttu-id="534d7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="534d7-152">DateTimeOffset</span></span>|<span data-ttu-id="534d7-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="534d7-153">DateTime the object was created.</span></span> <span data-ttu-id="534d7-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-155">description</span><span class="sxs-lookup"><span data-stu-id="534d7-155">description</span></span>|<span data-ttu-id="534d7-156">String</span><span class="sxs-lookup"><span data-stu-id="534d7-156">String</span></span>|<span data-ttu-id="534d7-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="534d7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="534d7-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="534d7-159">displayName</span></span>|<span data-ttu-id="534d7-160">String</span><span class="sxs-lookup"><span data-stu-id="534d7-160">String</span></span>|<span data-ttu-id="534d7-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="534d7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="534d7-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="534d7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-163">version</span><span class="sxs-lookup"><span data-stu-id="534d7-163">version</span></span>|<span data-ttu-id="534d7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="534d7-164">Int32</span></span>|<span data-ttu-id="534d7-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="534d7-165">Version of the device configuration.</span></span> <span data-ttu-id="534d7-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534d7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534d7-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="534d7-167">accountManagerPolicy</span></span>|[<span data-ttu-id="534d7-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="534d7-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="534d7-169">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="534d7-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="534d7-170">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="534d7-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="534d7-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="534d7-171">allowedAccounts</span></span>|[<span data-ttu-id="534d7-172">Шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="534d7-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="534d7-173">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="534d7-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="534d7-174">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="534d7-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="534d7-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="534d7-175">localStorage</span></span>|[<span data-ttu-id="534d7-176">Включение</span><span class="sxs-lookup"><span data-stu-id="534d7-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="534d7-177">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="534d7-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="534d7-178">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="534d7-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="534d7-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="534d7-179">allowLocalStorage</span></span>|<span data-ttu-id="534d7-180">Логический</span><span class="sxs-lookup"><span data-stu-id="534d7-180">Boolean</span></span>|<span data-ttu-id="534d7-181">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="534d7-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="534d7-182">Сетаккаунтманажер</span><span class="sxs-lookup"><span data-stu-id="534d7-182">setAccountManager</span></span>|[<span data-ttu-id="534d7-183">Включение</span><span class="sxs-lookup"><span data-stu-id="534d7-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="534d7-184">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="534d7-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="534d7-185">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="534d7-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="534d7-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="534d7-186">disableAccountManager</span></span>|<span data-ttu-id="534d7-187">Логический</span><span class="sxs-lookup"><span data-stu-id="534d7-187">Boolean</span></span>|<span data-ttu-id="534d7-188">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="534d7-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="534d7-189">СетедуполиЦиес</span><span class="sxs-lookup"><span data-stu-id="534d7-189">setEduPolicies</span></span>|[<span data-ttu-id="534d7-190">Включение</span><span class="sxs-lookup"><span data-stu-id="534d7-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="534d7-191">Указывает, следует ли включать и отключать/не настраивать общие политики среды по умолчанию для образовательных учреждений.</span><span class="sxs-lookup"><span data-stu-id="534d7-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="534d7-192">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="534d7-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="534d7-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="534d7-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="534d7-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="534d7-194">disableEduPolicies</span></span>|<span data-ttu-id="534d7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="534d7-195">Boolean</span></span>|<span data-ttu-id="534d7-196">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="534d7-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="534d7-197">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="534d7-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="534d7-198">СетповерполиЦиес</span><span class="sxs-lookup"><span data-stu-id="534d7-198">setPowerPolicies</span></span>|[<span data-ttu-id="534d7-199">Включение</span><span class="sxs-lookup"><span data-stu-id="534d7-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="534d7-200">Указывает, следует ли включать или отключать политики управления питанием общих ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="534d7-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="534d7-201">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="534d7-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="534d7-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="534d7-202">disablePowerPolicies</span></span>|<span data-ttu-id="534d7-203">Логический</span><span class="sxs-lookup"><span data-stu-id="534d7-203">Boolean</span></span>|<span data-ttu-id="534d7-204">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="534d7-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="534d7-205">Сигнинонресуме</span><span class="sxs-lookup"><span data-stu-id="534d7-205">signInOnResume</span></span>|[<span data-ttu-id="534d7-206">Включение</span><span class="sxs-lookup"><span data-stu-id="534d7-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="534d7-207">Задает требование для входа в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="534d7-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="534d7-208">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="534d7-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="534d7-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="534d7-209">disableSignInOnResume</span></span>|<span data-ttu-id="534d7-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="534d7-210">Boolean</span></span>|<span data-ttu-id="534d7-211">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="534d7-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="534d7-212">enabled</span><span class="sxs-lookup"><span data-stu-id="534d7-212">enabled</span></span>|<span data-ttu-id="534d7-213">Логический</span><span class="sxs-lookup"><span data-stu-id="534d7-213">Boolean</span></span>|<span data-ttu-id="534d7-214">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="534d7-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="534d7-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="534d7-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="534d7-216">Int32</span><span class="sxs-lookup"><span data-stu-id="534d7-216">Int32</span></span>|<span data-ttu-id="534d7-217">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="534d7-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="534d7-218">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="534d7-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="534d7-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="534d7-219">kioskAppDisplayName</span></span>|<span data-ttu-id="534d7-220">String</span><span class="sxs-lookup"><span data-stu-id="534d7-220">String</span></span>|<span data-ttu-id="534d7-221">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="534d7-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="534d7-222">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="534d7-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="534d7-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="534d7-223">kioskAppUserModelId</span></span>|<span data-ttu-id="534d7-224">String</span><span class="sxs-lookup"><span data-stu-id="534d7-224">String</span></span>|<span data-ttu-id="534d7-225">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="534d7-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="534d7-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="534d7-226">maintenanceStartTime</span></span>|<span data-ttu-id="534d7-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="534d7-227">TimeOfDay</span></span>|<span data-ttu-id="534d7-228">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="534d7-228">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="534d7-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="534d7-229">Response</span></span>
<span data-ttu-id="534d7-230">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="534d7-230">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="534d7-231">Пример</span><span class="sxs-lookup"><span data-stu-id="534d7-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="534d7-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="534d7-232">Request</span></span>
<span data-ttu-id="534d7-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="534d7-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1114

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
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="534d7-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="534d7-234">Response</span></span>
<span data-ttu-id="534d7-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="534d7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1286

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
  "maintenanceStartTime": "11:59:24.7240000"
}
```




