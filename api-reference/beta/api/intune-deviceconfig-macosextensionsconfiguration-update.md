---
title: Обновление Макосекстенсионсконфигуратион
description: Обновление свойств объекта Макосекстенсионсконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c852c56daac83609ac044d4c087dc6fc88752a1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315395"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="1c1af-103">Обновление Макосекстенсионсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1c1af-103">Update macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="1c1af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c1af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c1af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c1af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c1af-106">Обновление свойств объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1c1af-106">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c1af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c1af-107">Prerequisites</span></span>
<span data-ttu-id="1c1af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c1af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c1af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c1af-110">Permission type</span></span>|<span data-ttu-id="1c1af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c1af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c1af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c1af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c1af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c1af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c1af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c1af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c1af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c1af-115">Not supported.</span></span>|
|<span data-ttu-id="1c1af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c1af-116">Application</span></span>|<span data-ttu-id="1c1af-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c1af-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c1af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c1af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1c1af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c1af-119">Request headers</span></span>
|<span data-ttu-id="1c1af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c1af-120">Header</span></span>|<span data-ttu-id="1c1af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1c1af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c1af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c1af-122">Authorization</span></span>|<span data-ttu-id="1c1af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c1af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c1af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1c1af-124">Accept</span></span>|<span data-ttu-id="1c1af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c1af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c1af-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c1af-126">Request body</span></span>
<span data-ttu-id="1c1af-127">В тексте запроса добавьте представление объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c1af-127">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="1c1af-128">В следующей таблице приведены свойства, необходимые при создании [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-128">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="1c1af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c1af-129">Property</span></span>|<span data-ttu-id="1c1af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1c1af-130">Type</span></span>|<span data-ttu-id="1c1af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1c1af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c1af-132">id</span><span class="sxs-lookup"><span data-stu-id="1c1af-132">id</span></span>|<span data-ttu-id="1c1af-133">String</span><span class="sxs-lookup"><span data-stu-id="1c1af-133">String</span></span>|<span data-ttu-id="1c1af-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c1af-134">Key of the entity.</span></span> <span data-ttu-id="1c1af-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c1af-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1c1af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c1af-137">DateTimeOffset</span></span>|<span data-ttu-id="1c1af-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1c1af-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1c1af-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c1af-140">roleScopeTagIds</span></span>|<span data-ttu-id="1c1af-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1c1af-141">String collection</span></span>|<span data-ttu-id="1c1af-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1c1af-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c1af-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1c1af-144">supportsScopeTags</span></span>|<span data-ttu-id="1c1af-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1af-145">Boolean</span></span>|<span data-ttu-id="1c1af-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1c1af-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c1af-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1c1af-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c1af-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1c1af-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c1af-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c1af-149">This property is read-only.</span></span> <span data-ttu-id="1c1af-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1c1af-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1c1af-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1c1af-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1c1af-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1c1af-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1c1af-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1c1af-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1c1af-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1c1af-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1c1af-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1c1af-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1c1af-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1c1af-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1c1af-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1c1af-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1c1af-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1c1af-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1c1af-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c1af-163">createdDateTime</span></span>|<span data-ttu-id="1c1af-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c1af-164">DateTimeOffset</span></span>|<span data-ttu-id="1c1af-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1c1af-165">DateTime the object was created.</span></span> <span data-ttu-id="1c1af-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-167">description</span><span class="sxs-lookup"><span data-stu-id="1c1af-167">description</span></span>|<span data-ttu-id="1c1af-168">String</span><span class="sxs-lookup"><span data-stu-id="1c1af-168">String</span></span>|<span data-ttu-id="1c1af-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c1af-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c1af-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1c1af-171">displayName</span></span>|<span data-ttu-id="1c1af-172">Строка</span><span class="sxs-lookup"><span data-stu-id="1c1af-172">String</span></span>|<span data-ttu-id="1c1af-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c1af-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c1af-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-175">version</span><span class="sxs-lookup"><span data-stu-id="1c1af-175">version</span></span>|<span data-ttu-id="1c1af-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1c1af-176">Int32</span></span>|<span data-ttu-id="1c1af-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c1af-177">Version of the device configuration.</span></span> <span data-ttu-id="1c1af-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c1af-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c1af-179">кернелекстенсионоверридесалловед</span><span class="sxs-lookup"><span data-stu-id="1c1af-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="1c1af-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1af-180">Boolean</span></span>|<span data-ttu-id="1c1af-181">Если задано значение true, пользователи могут утверждать дополнительные расширения ядра, не разрешенные профилями конфигураций.</span><span class="sxs-lookup"><span data-stu-id="1c1af-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="1c1af-182">кернелекстенсионалловедтеамидентифиерс</span><span class="sxs-lookup"><span data-stu-id="1c1af-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="1c1af-183">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1c1af-183">String collection</span></span>|<span data-ttu-id="1c1af-184">Все расширения ядра, подписанные с помощью идентификаторов команд в этом списке, могут быть загружены.</span><span class="sxs-lookup"><span data-stu-id="1c1af-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="1c1af-185">кернелекстенсионсалловед</span><span class="sxs-lookup"><span data-stu-id="1c1af-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="1c1af-186">Коллекция [макоскернелекстенсион](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="1c1af-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="1c1af-187">Список расширений ядра, которые будут разрешены для загрузки.</span><span class="sxs-lookup"><span data-stu-id="1c1af-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="1c1af-188">.</span><span class="sxs-lookup"><span data-stu-id="1c1af-188"></span></span> <span data-ttu-id="1c1af-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1c1af-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1c1af-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c1af-190">Response</span></span>
<span data-ttu-id="1c1af-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c1af-191">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c1af-192">Пример</span><span class="sxs-lookup"><span data-stu-id="1c1af-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c1af-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c1af-193">Request</span></span>
<span data-ttu-id="1c1af-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c1af-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1383

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="1c1af-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c1af-195">Response</span></span>
<span data-ttu-id="1c1af-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c1af-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1555

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
  ]
}
```






