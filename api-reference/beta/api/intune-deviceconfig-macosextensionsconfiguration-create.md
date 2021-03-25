---
title: Создание macOSExtensionsConfiguration
description: Создайте новый объект macOSExtensionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4cc14e2015264f0d1e153c75f4bfdf65be34940d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151188"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="3656d-103">Создание macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="3656d-103">Create macOSExtensionsConfiguration</span></span>

<span data-ttu-id="3656d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3656d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3656d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3656d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3656d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3656d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3656d-107">Создайте [новый объект macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3656d-107">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3656d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3656d-108">Prerequisites</span></span>
<span data-ttu-id="3656d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3656d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3656d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3656d-111">Permission type</span></span>|<span data-ttu-id="3656d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3656d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3656d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3656d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3656d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3656d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3656d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3656d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3656d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3656d-116">Not supported.</span></span>|
|<span data-ttu-id="3656d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3656d-117">Application</span></span>|<span data-ttu-id="3656d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3656d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3656d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3656d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3656d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3656d-120">Request headers</span></span>
|<span data-ttu-id="3656d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3656d-121">Header</span></span>|<span data-ttu-id="3656d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3656d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3656d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3656d-123">Authorization</span></span>|<span data-ttu-id="3656d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3656d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3656d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3656d-125">Accept</span></span>|<span data-ttu-id="3656d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3656d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3656d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3656d-127">Request body</span></span>
<span data-ttu-id="3656d-128">В теле запроса предоставляем представление JSON для объекта macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3656d-128">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="3656d-129">В следующей таблице показаны свойства, необходимые при создании macOSExtensionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3656d-129">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="3656d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3656d-130">Property</span></span>|<span data-ttu-id="3656d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3656d-131">Type</span></span>|<span data-ttu-id="3656d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3656d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3656d-133">id</span><span class="sxs-lookup"><span data-stu-id="3656d-133">id</span></span>|<span data-ttu-id="3656d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3656d-134">String</span></span>|<span data-ttu-id="3656d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3656d-135">Key of the entity.</span></span> <span data-ttu-id="3656d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3656d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3656d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3656d-138">DateTimeOffset</span></span>|<span data-ttu-id="3656d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3656d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3656d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3656d-141">roleScopeTagIds</span></span>|<span data-ttu-id="3656d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3656d-142">String collection</span></span>|<span data-ttu-id="3656d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3656d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3656d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3656d-145">supportsScopeTags</span></span>|<span data-ttu-id="3656d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3656d-146">Boolean</span></span>|<span data-ttu-id="3656d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3656d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3656d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3656d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3656d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3656d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3656d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3656d-150">This property is read-only.</span></span> <span data-ttu-id="3656d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3656d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3656d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3656d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3656d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3656d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3656d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3656d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3656d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3656d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3656d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3656d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3656d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3656d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3656d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3656d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3656d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3656d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3656d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3656d-164">createdDateTime</span></span>|<span data-ttu-id="3656d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3656d-165">DateTimeOffset</span></span>|<span data-ttu-id="3656d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3656d-166">DateTime the object was created.</span></span> <span data-ttu-id="3656d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-168">description</span><span class="sxs-lookup"><span data-stu-id="3656d-168">description</span></span>|<span data-ttu-id="3656d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3656d-169">String</span></span>|<span data-ttu-id="3656d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3656d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3656d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3656d-172">displayName</span></span>|<span data-ttu-id="3656d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3656d-173">String</span></span>|<span data-ttu-id="3656d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3656d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3656d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-176">version</span><span class="sxs-lookup"><span data-stu-id="3656d-176">version</span></span>|<span data-ttu-id="3656d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3656d-177">Int32</span></span>|<span data-ttu-id="3656d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3656d-178">Version of the device configuration.</span></span> <span data-ttu-id="3656d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3656d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3656d-180">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="3656d-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="3656d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3656d-181">Boolean</span></span>|<span data-ttu-id="3656d-182">Если установлено, что это так, пользователи могут утверждать дополнительные расширения ядра, явно не разрешенные профилями конфигураций.</span><span class="sxs-lookup"><span data-stu-id="3656d-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="3656d-183">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="3656d-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="3656d-184">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3656d-184">String collection</span></span>|<span data-ttu-id="3656d-185">Все расширения ядра, действительно подписанные идентификаторами группы в этом списке, будут разрешены для загрузки.</span><span class="sxs-lookup"><span data-stu-id="3656d-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="3656d-186">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="3656d-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="3656d-187">[коллекция macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="3656d-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="3656d-188">Список расширений ядра, которые можно загрузить.</span><span class="sxs-lookup"><span data-stu-id="3656d-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="3656d-189">.</span><span class="sxs-lookup"><span data-stu-id="3656d-189">.</span></span> <span data-ttu-id="3656d-190">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3656d-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3656d-191">systemExtensionsBlockOverride</span><span class="sxs-lookup"><span data-stu-id="3656d-191">systemExtensionsBlockOverride</span></span>|<span data-ttu-id="3656d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="3656d-192">Boolean</span></span>|<span data-ttu-id="3656d-193">Получает или задает, разрешить ли пользователю утверждать дополнительные расширения системы, явно не разрешенные профилями конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3656d-193">Gets or sets whether to allow the user to approve additional system extensions not explicitly allowed by configuration profiles.</span></span>|
|<span data-ttu-id="3656d-194">systemExtensionsAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="3656d-194">systemExtensionsAllowedTeamIdentifiers</span></span>|<span data-ttu-id="3656d-195">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3656d-195">String collection</span></span>|<span data-ttu-id="3656d-196">Получает или задает список разрешенных идентификаторов группы.</span><span class="sxs-lookup"><span data-stu-id="3656d-196">Gets or sets a list of allowed team identifiers.</span></span> <span data-ttu-id="3656d-197">Любое расширение системы, подписанное с любым из указанных идентификаторов группы, будет утверждено.</span><span class="sxs-lookup"><span data-stu-id="3656d-197">Any system extension signed with any of the specified team identifiers will be approved.</span></span>|
|<span data-ttu-id="3656d-198">systemExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="3656d-198">systemExtensionsAllowed</span></span>|<span data-ttu-id="3656d-199">[коллекция macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md)</span><span class="sxs-lookup"><span data-stu-id="3656d-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) collection</span></span>|<span data-ttu-id="3656d-200">Получает или задает список разрешенных расширений системы macOS.</span><span class="sxs-lookup"><span data-stu-id="3656d-200">Gets or sets a list of allowed macOS system extensions.</span></span> <span data-ttu-id="3656d-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3656d-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3656d-202">systemExtensionsAllowedTypes</span><span class="sxs-lookup"><span data-stu-id="3656d-202">systemExtensionsAllowedTypes</span></span>|<span data-ttu-id="3656d-203">[коллекция macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)</span><span class="sxs-lookup"><span data-stu-id="3656d-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) collection</span></span>|<span data-ttu-id="3656d-204">Получает или задает список разрешенных типов расширения системы macOS.</span><span class="sxs-lookup"><span data-stu-id="3656d-204">Gets or sets a list of allowed macOS system extension types.</span></span> <span data-ttu-id="3656d-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3656d-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3656d-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="3656d-206">Response</span></span>
<span data-ttu-id="3656d-207">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3656d-207">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3656d-208">Пример</span><span class="sxs-lookup"><span data-stu-id="3656d-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="3656d-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="3656d-209">Request</span></span>
<span data-ttu-id="3656d-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3656d-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1965

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3656d-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="3656d-211">Response</span></span>
<span data-ttu-id="3656d-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3656d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2137

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```




