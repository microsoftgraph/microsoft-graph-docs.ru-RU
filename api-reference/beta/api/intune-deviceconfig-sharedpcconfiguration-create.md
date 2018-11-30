---
title: Create sharedPCConfiguration
description: Создание объекта sharedPCConfiguration.
ms.openlocfilehash: 2cd92e4e2d3147cccbd9099d16ecfaaac0c8c656
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075892"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="d6e53-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6e53-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="d6e53-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6e53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6e53-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6e53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6e53-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6e53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6e53-107">Создание объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-107">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6e53-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d6e53-108">Prerequisites</span></span>
<span data-ttu-id="d6e53-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6e53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6e53-111">Permission type</span></span>|<span data-ttu-id="d6e53-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6e53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6e53-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6e53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6e53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6e53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6e53-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6e53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6e53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6e53-116">Not supported.</span></span>|
|<span data-ttu-id="d6e53-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6e53-117">Application</span></span>|<span data-ttu-id="d6e53-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6e53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6e53-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6e53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6e53-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6e53-120">Request headers</span></span>
|<span data-ttu-id="d6e53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6e53-121">Header</span></span>|<span data-ttu-id="d6e53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6e53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6e53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6e53-123">Authorization</span></span>|<span data-ttu-id="d6e53-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d6e53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6e53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6e53-125">Accept</span></span>|<span data-ttu-id="d6e53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6e53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6e53-127">Request body</span></span>
<span data-ttu-id="d6e53-128">В тексте запроса добавьте представление объекта sharedPCConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6e53-128">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="d6e53-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6e53-129">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="d6e53-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6e53-130">Property</span></span>|<span data-ttu-id="d6e53-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6e53-131">Type</span></span>|<span data-ttu-id="d6e53-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6e53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6e53-133">id</span><span class="sxs-lookup"><span data-stu-id="d6e53-133">id</span></span>|<span data-ttu-id="d6e53-134">String</span><span class="sxs-lookup"><span data-stu-id="d6e53-134">String</span></span>|<span data-ttu-id="d6e53-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d6e53-135">Key of the entity.</span></span> <span data-ttu-id="d6e53-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6e53-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d6e53-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6e53-138">DateTimeOffset</span></span>|<span data-ttu-id="d6e53-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d6e53-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d6e53-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6e53-141">roleScopeTagIds</span></span>|<span data-ttu-id="d6e53-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6e53-142">String collection</span></span>|<span data-ttu-id="d6e53-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d6e53-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6e53-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d6e53-145">supportsScopeTags</span></span>|<span data-ttu-id="d6e53-146">Логический</span><span class="sxs-lookup"><span data-stu-id="d6e53-146">Boolean</span></span>|<span data-ttu-id="d6e53-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="d6e53-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d6e53-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="d6e53-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d6e53-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d6e53-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d6e53-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d6e53-150">This property is read-only.</span></span> <span data-ttu-id="d6e53-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6e53-152">createdDateTime</span></span>|<span data-ttu-id="d6e53-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6e53-153">DateTimeOffset</span></span>|<span data-ttu-id="d6e53-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d6e53-154">DateTime the object was created.</span></span> <span data-ttu-id="d6e53-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-156">описание</span><span class="sxs-lookup"><span data-stu-id="d6e53-156">description</span></span>|<span data-ttu-id="d6e53-157">String</span><span class="sxs-lookup"><span data-stu-id="d6e53-157">String</span></span>|<span data-ttu-id="d6e53-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d6e53-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6e53-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d6e53-160">displayName</span></span>|<span data-ttu-id="d6e53-161">String</span><span class="sxs-lookup"><span data-stu-id="d6e53-161">String</span></span>|<span data-ttu-id="d6e53-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d6e53-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6e53-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6e53-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-164">version</span><span class="sxs-lookup"><span data-stu-id="d6e53-164">version</span></span>|<span data-ttu-id="d6e53-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d6e53-165">Int32</span></span>|<span data-ttu-id="d6e53-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d6e53-166">Version of the device configuration.</span></span> <span data-ttu-id="d6e53-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6e53-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6e53-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="d6e53-168">accountManagerPolicy</span></span>|[<span data-ttu-id="d6e53-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="d6e53-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="d6e53-170">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="d6e53-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="d6e53-171">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="d6e53-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="d6e53-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="d6e53-172">allowedAccounts</span></span>|[<span data-ttu-id="d6e53-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="d6e53-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="d6e53-174">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="d6e53-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="d6e53-175">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="d6e53-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="d6e53-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="d6e53-176">localStorage</span></span>|[<span data-ttu-id="d6e53-177">Включение</span><span class="sxs-lookup"><span data-stu-id="d6e53-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d6e53-178">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="d6e53-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="d6e53-179">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d6e53-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d6e53-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="d6e53-180">allowLocalStorage</span></span>|<span data-ttu-id="d6e53-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6e53-181">Boolean</span></span>|<span data-ttu-id="d6e53-182">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="d6e53-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="d6e53-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="d6e53-183">setAccountManager</span></span>|[<span data-ttu-id="d6e53-184">Включение</span><span class="sxs-lookup"><span data-stu-id="d6e53-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d6e53-185">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="d6e53-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="d6e53-186">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d6e53-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d6e53-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="d6e53-187">disableAccountManager</span></span>|<span data-ttu-id="d6e53-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6e53-188">Boolean</span></span>|<span data-ttu-id="d6e53-189">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="d6e53-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="d6e53-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="d6e53-190">setEduPolicies</span></span>|[<span data-ttu-id="d6e53-191">Включение</span><span class="sxs-lookup"><span data-stu-id="d6e53-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d6e53-192">Указывает ли политики по умолчанию общих ПК education среды должен быть включен или отключен или не настроен.</span><span class="sxs-lookup"><span data-stu-id="d6e53-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="d6e53-193">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="d6e53-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="d6e53-194">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d6e53-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d6e53-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="d6e53-195">disableEduPolicies</span></span>|<span data-ttu-id="d6e53-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6e53-196">Boolean</span></span>|<span data-ttu-id="d6e53-197">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="d6e53-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="d6e53-198">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="d6e53-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="d6e53-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="d6e53-199">setPowerPolicies</span></span>|[<span data-ttu-id="d6e53-200">Включение</span><span class="sxs-lookup"><span data-stu-id="d6e53-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d6e53-201">Указывает, будет ли политики по умолчанию общих PC power должен быть отключен.</span><span class="sxs-lookup"><span data-stu-id="d6e53-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="d6e53-202">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d6e53-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d6e53-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="d6e53-203">disablePowerPolicies</span></span>|<span data-ttu-id="d6e53-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6e53-204">Boolean</span></span>|<span data-ttu-id="d6e53-205">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="d6e53-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="d6e53-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="d6e53-206">signInOnResume</span></span>|[<span data-ttu-id="d6e53-207">Включение</span><span class="sxs-lookup"><span data-stu-id="d6e53-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d6e53-208">Определяет требования для входа в каждый раз, когда устройство выходит из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="d6e53-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="d6e53-209">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d6e53-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d6e53-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="d6e53-210">disableSignInOnResume</span></span>|<span data-ttu-id="d6e53-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6e53-211">Boolean</span></span>|<span data-ttu-id="d6e53-212">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="d6e53-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="d6e53-213">enabled</span><span class="sxs-lookup"><span data-stu-id="d6e53-213">enabled</span></span>|<span data-ttu-id="d6e53-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6e53-214">Boolean</span></span>|<span data-ttu-id="d6e53-215">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="d6e53-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="d6e53-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="d6e53-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="d6e53-217">Int32</span><span class="sxs-lookup"><span data-stu-id="d6e53-217">Int32</span></span>|<span data-ttu-id="d6e53-218">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="d6e53-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="d6e53-219">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="d6e53-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="d6e53-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6e53-220">kioskAppDisplayName</span></span>|<span data-ttu-id="d6e53-221">String</span><span class="sxs-lookup"><span data-stu-id="d6e53-221">String</span></span>|<span data-ttu-id="d6e53-222">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="d6e53-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="d6e53-223">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="d6e53-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="d6e53-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="d6e53-224">kioskAppUserModelId</span></span>|<span data-ttu-id="d6e53-225">String</span><span class="sxs-lookup"><span data-stu-id="d6e53-225">String</span></span>|<span data-ttu-id="d6e53-226">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="d6e53-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="d6e53-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="d6e53-227">maintenanceStartTime</span></span>|<span data-ttu-id="d6e53-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d6e53-228">TimeOfDay</span></span>|<span data-ttu-id="d6e53-229">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="d6e53-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="d6e53-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6e53-230">Response</span></span>
<span data-ttu-id="d6e53-231">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d6e53-231">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6e53-232">Пример</span><span class="sxs-lookup"><span data-stu-id="d6e53-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6e53-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6e53-233">Request</span></span>
<span data-ttu-id="d6e53-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6e53-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1179

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "allowedAccounts": "domain",
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

### <a name="response"></a><span data-ttu-id="d6e53-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6e53-235">Response</span></span>
<span data-ttu-id="d6e53-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d6e53-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1287

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
  "allowedAccounts": "domain",
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





