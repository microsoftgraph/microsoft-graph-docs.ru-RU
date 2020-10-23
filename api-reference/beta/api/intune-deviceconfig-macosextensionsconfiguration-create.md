---
title: Создание Макосекстенсионсконфигуратион
description: Создание нового объекта Макосекстенсионсконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db25ad21995465f941c1a31e333779c3d6e1f303
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689757"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="5b76f-103">Создание Макосекстенсионсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5b76f-103">Create macOSExtensionsConfiguration</span></span>

<span data-ttu-id="5b76f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b76f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b76f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b76f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b76f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b76f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b76f-107">Создание нового объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5b76f-107">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b76f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b76f-108">Prerequisites</span></span>
<span data-ttu-id="5b76f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b76f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b76f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b76f-111">Permission type</span></span>|<span data-ttu-id="5b76f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b76f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b76f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b76f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b76f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b76f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b76f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b76f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b76f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b76f-116">Not supported.</span></span>|
|<span data-ttu-id="5b76f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b76f-117">Application</span></span>|<span data-ttu-id="5b76f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b76f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b76f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b76f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5b76f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b76f-120">Request headers</span></span>
|<span data-ttu-id="5b76f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b76f-121">Header</span></span>|<span data-ttu-id="5b76f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b76f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b76f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b76f-123">Authorization</span></span>|<span data-ttu-id="5b76f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b76f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b76f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b76f-125">Accept</span></span>|<span data-ttu-id="5b76f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b76f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b76f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b76f-127">Request body</span></span>
<span data-ttu-id="5b76f-128">В тексте запроса добавьте представление объекта Макосекстенсионсконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b76f-128">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="5b76f-129">В следующей таблице приведены свойства, необходимые при создании Макосекстенсионсконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="5b76f-129">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="5b76f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b76f-130">Property</span></span>|<span data-ttu-id="5b76f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b76f-131">Type</span></span>|<span data-ttu-id="5b76f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b76f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b76f-133">id</span><span class="sxs-lookup"><span data-stu-id="5b76f-133">id</span></span>|<span data-ttu-id="5b76f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5b76f-134">String</span></span>|<span data-ttu-id="5b76f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b76f-135">Key of the entity.</span></span> <span data-ttu-id="5b76f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b76f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5b76f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b76f-138">DateTimeOffset</span></span>|<span data-ttu-id="5b76f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5b76f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5b76f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b76f-141">roleScopeTagIds</span></span>|<span data-ttu-id="5b76f-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5b76f-142">String collection</span></span>|<span data-ttu-id="5b76f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5b76f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b76f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5b76f-145">supportsScopeTags</span></span>|<span data-ttu-id="5b76f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5b76f-146">Boolean</span></span>|<span data-ttu-id="5b76f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5b76f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5b76f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5b76f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5b76f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5b76f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5b76f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b76f-150">This property is read-only.</span></span> <span data-ttu-id="5b76f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5b76f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5b76f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5b76f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5b76f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b76f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5b76f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5b76f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5b76f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5b76f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5b76f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b76f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5b76f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5b76f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5b76f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5b76f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5b76f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b76f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5b76f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b76f-164">createdDateTime</span></span>|<span data-ttu-id="5b76f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b76f-165">DateTimeOffset</span></span>|<span data-ttu-id="5b76f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5b76f-166">DateTime the object was created.</span></span> <span data-ttu-id="5b76f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-168">description</span><span class="sxs-lookup"><span data-stu-id="5b76f-168">description</span></span>|<span data-ttu-id="5b76f-169">Строка</span><span class="sxs-lookup"><span data-stu-id="5b76f-169">String</span></span>|<span data-ttu-id="5b76f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b76f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b76f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5b76f-172">displayName</span></span>|<span data-ttu-id="5b76f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="5b76f-173">String</span></span>|<span data-ttu-id="5b76f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b76f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b76f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-176">version</span><span class="sxs-lookup"><span data-stu-id="5b76f-176">version</span></span>|<span data-ttu-id="5b76f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5b76f-177">Int32</span></span>|<span data-ttu-id="5b76f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b76f-178">Version of the device configuration.</span></span> <span data-ttu-id="5b76f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b76f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b76f-180">кернелекстенсионоверридесалловед</span><span class="sxs-lookup"><span data-stu-id="5b76f-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="5b76f-181">Логический</span><span class="sxs-lookup"><span data-stu-id="5b76f-181">Boolean</span></span>|<span data-ttu-id="5b76f-182">Если задано значение true, пользователи могут утверждать дополнительные расширения ядра, не разрешенные профилями конфигураций.</span><span class="sxs-lookup"><span data-stu-id="5b76f-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="5b76f-183">кернелекстенсионалловедтеамидентифиерс</span><span class="sxs-lookup"><span data-stu-id="5b76f-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="5b76f-184">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5b76f-184">String collection</span></span>|<span data-ttu-id="5b76f-185">Все расширения ядра, подписанные с помощью идентификаторов команд в этом списке, могут быть загружены.</span><span class="sxs-lookup"><span data-stu-id="5b76f-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="5b76f-186">кернелекстенсионсалловед</span><span class="sxs-lookup"><span data-stu-id="5b76f-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="5b76f-187">Коллекция [макоскернелекстенсион](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="5b76f-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="5b76f-188">Список расширений ядра, которые будут разрешены для загрузки.</span><span class="sxs-lookup"><span data-stu-id="5b76f-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="5b76f-189">.</span><span class="sxs-lookup"><span data-stu-id="5b76f-189">.</span></span> <span data-ttu-id="5b76f-190">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5b76f-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5b76f-191">системекстенсионсблокковерриде</span><span class="sxs-lookup"><span data-stu-id="5b76f-191">systemExtensionsBlockOverride</span></span>|<span data-ttu-id="5b76f-192">Логический</span><span class="sxs-lookup"><span data-stu-id="5b76f-192">Boolean</span></span>|<span data-ttu-id="5b76f-193">Получает или задает значение, указывающее, следует ли разрешить пользователю утверждать дополнительные системные расширения, которые явно не разрешены профилями конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5b76f-193">Gets or sets whether to allow the user to approve additional system extensions not explicitly allowed by configuration profiles.</span></span>|
|<span data-ttu-id="5b76f-194">системекстенсионсалловедтеамидентифиерс</span><span class="sxs-lookup"><span data-stu-id="5b76f-194">systemExtensionsAllowedTeamIdentifiers</span></span>|<span data-ttu-id="5b76f-195">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5b76f-195">String collection</span></span>|<span data-ttu-id="5b76f-196">Получает или задает список разрешенных идентификаторов групп.</span><span class="sxs-lookup"><span data-stu-id="5b76f-196">Gets or sets a list of allowed team identifiers.</span></span> <span data-ttu-id="5b76f-197">Все системные расширения, подписанные с помощью любого из указанных идентификаторов, будут утверждены.</span><span class="sxs-lookup"><span data-stu-id="5b76f-197">Any system extension signed with any of the specified team identifiers will be approved.</span></span>|
|<span data-ttu-id="5b76f-198">системекстенсионсалловед</span><span class="sxs-lookup"><span data-stu-id="5b76f-198">systemExtensionsAllowed</span></span>|<span data-ttu-id="5b76f-199">Коллекция [макоссистемекстенсион](../resources/intune-deviceconfig-macossystemextension.md)</span><span class="sxs-lookup"><span data-stu-id="5b76f-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) collection</span></span>|<span data-ttu-id="5b76f-200">Получает или задает список разрешенных расширений системы macOS.</span><span class="sxs-lookup"><span data-stu-id="5b76f-200">Gets or sets a list of allowed macOS system extensions.</span></span> <span data-ttu-id="5b76f-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5b76f-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5b76f-202">системекстенсионсалловедтипес</span><span class="sxs-lookup"><span data-stu-id="5b76f-202">systemExtensionsAllowedTypes</span></span>|<span data-ttu-id="5b76f-203">Коллекция [макоссистемекстенсионтипемаппинг](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)</span><span class="sxs-lookup"><span data-stu-id="5b76f-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) collection</span></span>|<span data-ttu-id="5b76f-204">Получает или задает список разрешенных типов расширений системы macOS.</span><span class="sxs-lookup"><span data-stu-id="5b76f-204">Gets or sets a list of allowed macOS system extension types.</span></span> <span data-ttu-id="5b76f-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5b76f-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5b76f-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b76f-206">Response</span></span>
<span data-ttu-id="5b76f-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b76f-207">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b76f-208">Пример</span><span class="sxs-lookup"><span data-stu-id="5b76f-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b76f-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b76f-209">Request</span></span>
<span data-ttu-id="5b76f-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b76f-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b76f-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b76f-211">Response</span></span>
<span data-ttu-id="5b76f-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b76f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





