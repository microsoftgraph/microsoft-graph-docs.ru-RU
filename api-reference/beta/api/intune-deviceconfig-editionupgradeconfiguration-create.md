---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
ms.openlocfilehash: 19dab90bafd328980d3083d370c5ac5bb9c5bb5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079328"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="6f8c5-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f8c5-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="6f8c5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f8c5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f8c5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f8c5-107">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f8c5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f8c5-108">Prerequisites</span></span>
<span data-ttu-id="6f8c5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f8c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f8c5-111">Permission type</span></span>|<span data-ttu-id="6f8c5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f8c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f8c5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f8c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f8c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f8c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f8c5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f8c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f8c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-116">Not supported.</span></span>|
|<span data-ttu-id="6f8c5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f8c5-117">Application</span></span>|<span data-ttu-id="6f8c5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f8c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f8c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f8c5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f8c5-120">Request headers</span></span>
|<span data-ttu-id="6f8c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f8c5-121">Header</span></span>|<span data-ttu-id="6f8c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f8c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f8c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f8c5-123">Authorization</span></span>|<span data-ttu-id="6f8c5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f8c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f8c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f8c5-125">Accept</span></span>|<span data-ttu-id="6f8c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f8c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f8c5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f8c5-127">Request body</span></span>
<span data-ttu-id="6f8c5-128">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="6f8c5-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="6f8c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f8c5-130">Property</span></span>|<span data-ttu-id="6f8c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f8c5-131">Type</span></span>|<span data-ttu-id="6f8c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f8c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f8c5-133">id</span><span class="sxs-lookup"><span data-stu-id="6f8c5-133">id</span></span>|<span data-ttu-id="6f8c5-134">String</span><span class="sxs-lookup"><span data-stu-id="6f8c5-134">String</span></span>|<span data-ttu-id="6f8c5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-135">Key of the entity.</span></span> <span data-ttu-id="6f8c5-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f8c5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f8c5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f8c5-138">DateTimeOffset</span></span>|<span data-ttu-id="6f8c5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f8c5-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f8c5-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f8c5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f8c5-142">String collection</span></span>|<span data-ttu-id="6f8c5-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f8c5-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f8c5-145">supportsScopeTags</span></span>|<span data-ttu-id="6f8c5-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6f8c5-146">Boolean</span></span>|<span data-ttu-id="6f8c5-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f8c5-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f8c5-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f8c5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-150">This property is read-only.</span></span> <span data-ttu-id="6f8c5-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f8c5-152">createdDateTime</span></span>|<span data-ttu-id="6f8c5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f8c5-153">DateTimeOffset</span></span>|<span data-ttu-id="6f8c5-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-154">DateTime the object was created.</span></span> <span data-ttu-id="6f8c5-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-156">описание</span><span class="sxs-lookup"><span data-stu-id="6f8c5-156">description</span></span>|<span data-ttu-id="6f8c5-157">String</span><span class="sxs-lookup"><span data-stu-id="6f8c5-157">String</span></span>|<span data-ttu-id="6f8c5-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f8c5-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6f8c5-160">displayName</span></span>|<span data-ttu-id="6f8c5-161">String</span><span class="sxs-lookup"><span data-stu-id="6f8c5-161">String</span></span>|<span data-ttu-id="6f8c5-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f8c5-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-164">version</span><span class="sxs-lookup"><span data-stu-id="6f8c5-164">version</span></span>|<span data-ttu-id="6f8c5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6f8c5-165">Int32</span></span>|<span data-ttu-id="6f8c5-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-166">Version of the device configuration.</span></span> <span data-ttu-id="6f8c5-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8c5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8c5-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="6f8c5-168">licenseType</span></span>|[<span data-ttu-id="6f8c5-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="6f8c5-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="6f8c5-170">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="6f8c5-171">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="6f8c5-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="6f8c5-172">targetEdition</span></span>|[<span data-ttu-id="6f8c5-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="6f8c5-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="6f8c5-174">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="6f8c5-175">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="6f8c5-176">license</span><span class="sxs-lookup"><span data-stu-id="6f8c5-176">license</span></span>|<span data-ttu-id="6f8c5-177">String</span><span class="sxs-lookup"><span data-stu-id="6f8c5-177">String</span></span>|<span data-ttu-id="6f8c5-178">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="6f8c5-179">productKey</span><span class="sxs-lookup"><span data-stu-id="6f8c5-179">productKey</span></span>|<span data-ttu-id="6f8c5-180">String</span><span class="sxs-lookup"><span data-stu-id="6f8c5-180">String</span></span>|<span data-ttu-id="6f8c5-181">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="6f8c5-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="6f8c5-182">windowsSMode</span></span>|[<span data-ttu-id="6f8c5-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f8c5-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="6f8c5-184">Конфигурация S.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-184">S mode configuration.</span></span> <span data-ttu-id="6f8c5-185">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="6f8c5-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f8c5-186">Response</span></span>
<span data-ttu-id="6f8c5-187">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-187">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f8c5-188">Пример</span><span class="sxs-lookup"><span data-stu-id="6f8c5-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f8c5-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f8c5-189">Request</span></span>
<span data-ttu-id="6f8c5-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f8c5-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="6f8c5-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f8c5-191">Response</span></span>
<span data-ttu-id="6f8c5-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6f8c5-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 603

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```





