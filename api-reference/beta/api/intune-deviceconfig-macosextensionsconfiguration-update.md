---
title: Обновление Макосекстенсионсконфигуратион
description: Обновление свойств объекта Макосекстенсионсконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ad2570183edbf544b465067370b079ddf55c8b0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179553"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="c3564-103">Обновление Макосекстенсионсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c3564-103">Update macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="c3564-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3564-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3564-106">Обновление свойств объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c3564-106">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3564-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3564-107">Prerequisites</span></span>
<span data-ttu-id="c3564-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3564-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3564-110">Permission type</span></span>|<span data-ttu-id="c3564-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3564-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3564-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3564-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3564-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3564-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3564-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3564-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3564-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3564-115">Not supported.</span></span>|
|<span data-ttu-id="c3564-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3564-116">Application</span></span>|<span data-ttu-id="c3564-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3564-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3564-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3564-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c3564-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3564-119">Request headers</span></span>
|<span data-ttu-id="c3564-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3564-120">Header</span></span>|<span data-ttu-id="c3564-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c3564-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3564-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3564-122">Authorization</span></span>|<span data-ttu-id="c3564-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3564-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3564-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c3564-124">Accept</span></span>|<span data-ttu-id="c3564-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3564-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3564-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3564-126">Request body</span></span>
<span data-ttu-id="c3564-127">В тексте запроса добавьте представление объекта [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3564-127">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="c3564-128">В следующей таблице приведены свойства, необходимые при создании [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-128">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="c3564-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3564-129">Property</span></span>|<span data-ttu-id="c3564-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c3564-130">Type</span></span>|<span data-ttu-id="c3564-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c3564-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3564-132">id</span><span class="sxs-lookup"><span data-stu-id="c3564-132">id</span></span>|<span data-ttu-id="c3564-133">String</span><span class="sxs-lookup"><span data-stu-id="c3564-133">String</span></span>|<span data-ttu-id="c3564-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3564-134">Key of the entity.</span></span> <span data-ttu-id="c3564-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3564-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c3564-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3564-137">DateTimeOffset</span></span>|<span data-ttu-id="c3564-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c3564-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c3564-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3564-140">roleScopeTagIds</span></span>|<span data-ttu-id="c3564-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3564-141">String collection</span></span>|<span data-ttu-id="c3564-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c3564-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3564-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c3564-144">supportsScopeTags</span></span>|<span data-ttu-id="c3564-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c3564-145">Boolean</span></span>|<span data-ttu-id="c3564-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c3564-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c3564-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c3564-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c3564-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c3564-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c3564-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3564-149">This property is read-only.</span></span> <span data-ttu-id="c3564-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3564-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c3564-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3564-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c3564-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3564-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c3564-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3564-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c3564-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3564-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c3564-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3564-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c3564-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c3564-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c3564-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c3564-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c3564-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3564-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c3564-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3564-163">createdDateTime</span></span>|<span data-ttu-id="c3564-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3564-164">DateTimeOffset</span></span>|<span data-ttu-id="c3564-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c3564-165">DateTime the object was created.</span></span> <span data-ttu-id="c3564-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-167">description</span><span class="sxs-lookup"><span data-stu-id="c3564-167">description</span></span>|<span data-ttu-id="c3564-168">String</span><span class="sxs-lookup"><span data-stu-id="c3564-168">String</span></span>|<span data-ttu-id="c3564-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3564-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3564-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c3564-171">displayName</span></span>|<span data-ttu-id="c3564-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c3564-172">String</span></span>|<span data-ttu-id="c3564-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3564-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3564-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-175">version</span><span class="sxs-lookup"><span data-stu-id="c3564-175">version</span></span>|<span data-ttu-id="c3564-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c3564-176">Int32</span></span>|<span data-ttu-id="c3564-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3564-177">Version of the device configuration.</span></span> <span data-ttu-id="c3564-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3564-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3564-179">кернелекстенсионоверридесалловед</span><span class="sxs-lookup"><span data-stu-id="c3564-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="c3564-180">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c3564-180">Boolean</span></span>|<span data-ttu-id="c3564-181">Если задано значение true, пользователи могут утверждать дополнительные расширения ядра, не разрешенные профилями конфигураций.</span><span class="sxs-lookup"><span data-stu-id="c3564-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="c3564-182">кернелекстенсионалловедтеамидентифиерс</span><span class="sxs-lookup"><span data-stu-id="c3564-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="c3564-183">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3564-183">String collection</span></span>|<span data-ttu-id="c3564-184">Все расширения ядра, подписанные с помощью идентификаторов команд в этом списке, могут быть загружены.</span><span class="sxs-lookup"><span data-stu-id="c3564-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="c3564-185">кернелекстенсионсалловед</span><span class="sxs-lookup"><span data-stu-id="c3564-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="c3564-186">Коллекция [макоскернелекстенсион](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="c3564-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="c3564-187">Список расширений ядра, которые будут разрешены для загрузки.</span><span class="sxs-lookup"><span data-stu-id="c3564-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="c3564-188">.</span><span class="sxs-lookup"><span data-stu-id="c3564-188"></span></span> <span data-ttu-id="c3564-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c3564-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c3564-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3564-190">Response</span></span>
<span data-ttu-id="c3564-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3564-191">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3564-192">Пример</span><span class="sxs-lookup"><span data-stu-id="c3564-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3564-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3564-193">Request</span></span>
<span data-ttu-id="c3564-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3564-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3564-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3564-195">Response</span></span>
<span data-ttu-id="c3564-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3564-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




