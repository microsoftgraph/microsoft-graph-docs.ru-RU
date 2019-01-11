---
title: Обновление объекта editionUpgradeConfiguration
description: Обновление свойств объекта editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6cdc28cb5f00f197bea5d6efa23ea7b8d1859e31
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878143"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="a68b8-103">Обновление объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a68b8-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="a68b8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a68b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a68b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a68b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a68b8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a68b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a68b8-107">Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a68b8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a68b8-108">Prerequisites</span></span>
<span data-ttu-id="a68b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a68b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a68b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a68b8-111">Permission type</span></span>|<span data-ttu-id="a68b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a68b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a68b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a68b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a68b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a68b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a68b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a68b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a68b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a68b8-116">Not supported.</span></span>|
|<span data-ttu-id="a68b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a68b8-117">Application</span></span>|<span data-ttu-id="a68b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a68b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a68b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a68b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a68b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a68b8-120">Request headers</span></span>
|<span data-ttu-id="a68b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a68b8-121">Header</span></span>|<span data-ttu-id="a68b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a68b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a68b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a68b8-123">Authorization</span></span>|<span data-ttu-id="a68b8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a68b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a68b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a68b8-125">Accept</span></span>|<span data-ttu-id="a68b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a68b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a68b8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a68b8-127">Request body</span></span>
<span data-ttu-id="a68b8-128">В теле запроса добавьте представление объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a68b8-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="a68b8-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="a68b8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a68b8-130">Property</span></span>|<span data-ttu-id="a68b8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a68b8-131">Type</span></span>|<span data-ttu-id="a68b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a68b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a68b8-133">id</span><span class="sxs-lookup"><span data-stu-id="a68b8-133">id</span></span>|<span data-ttu-id="a68b8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a68b8-134">String</span></span>|<span data-ttu-id="a68b8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a68b8-135">Key of the entity.</span></span> <span data-ttu-id="a68b8-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a68b8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a68b8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a68b8-138">DateTimeOffset</span></span>|<span data-ttu-id="a68b8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a68b8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a68b8-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a68b8-141">roleScopeTagIds</span></span>|<span data-ttu-id="a68b8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a68b8-142">String collection</span></span>|<span data-ttu-id="a68b8-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a68b8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a68b8-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a68b8-145">supportsScopeTags</span></span>|<span data-ttu-id="a68b8-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a68b8-146">Boolean</span></span>|<span data-ttu-id="a68b8-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="a68b8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a68b8-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="a68b8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a68b8-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a68b8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a68b8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a68b8-150">This property is read-only.</span></span> <span data-ttu-id="a68b8-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a68b8-152">createdDateTime</span></span>|<span data-ttu-id="a68b8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a68b8-153">DateTimeOffset</span></span>|<span data-ttu-id="a68b8-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a68b8-154">DateTime the object was created.</span></span> <span data-ttu-id="a68b8-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-156">описание</span><span class="sxs-lookup"><span data-stu-id="a68b8-156">description</span></span>|<span data-ttu-id="a68b8-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a68b8-157">String</span></span>|<span data-ttu-id="a68b8-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a68b8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a68b8-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a68b8-160">displayName</span></span>|<span data-ttu-id="a68b8-161">Строка</span><span class="sxs-lookup"><span data-stu-id="a68b8-161">String</span></span>|<span data-ttu-id="a68b8-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a68b8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a68b8-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-164">version</span><span class="sxs-lookup"><span data-stu-id="a68b8-164">version</span></span>|<span data-ttu-id="a68b8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a68b8-165">Int32</span></span>|<span data-ttu-id="a68b8-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a68b8-166">Version of the device configuration.</span></span> <span data-ttu-id="a68b8-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a68b8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a68b8-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="a68b8-168">licenseType</span></span>|[<span data-ttu-id="a68b8-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="a68b8-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="a68b8-170">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="a68b8-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="a68b8-171">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a68b8-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="a68b8-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="a68b8-172">targetEdition</span></span>|[<span data-ttu-id="a68b8-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="a68b8-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="a68b8-174">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="a68b8-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="a68b8-175">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a68b8-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="a68b8-176">license</span><span class="sxs-lookup"><span data-stu-id="a68b8-176">license</span></span>|<span data-ttu-id="a68b8-177">String</span><span class="sxs-lookup"><span data-stu-id="a68b8-177">String</span></span>|<span data-ttu-id="a68b8-178">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="a68b8-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="a68b8-179">productKey</span><span class="sxs-lookup"><span data-stu-id="a68b8-179">productKey</span></span>|<span data-ttu-id="a68b8-180">String</span><span class="sxs-lookup"><span data-stu-id="a68b8-180">String</span></span>|<span data-ttu-id="a68b8-181">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="a68b8-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="a68b8-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="a68b8-182">windowsSMode</span></span>|[<span data-ttu-id="a68b8-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a68b8-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="a68b8-184">Конфигурация S.</span><span class="sxs-lookup"><span data-stu-id="a68b8-184">S mode configuration.</span></span> <span data-ttu-id="a68b8-185">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="a68b8-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="a68b8-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="a68b8-186">Response</span></span>
<span data-ttu-id="a68b8-187">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a68b8-187">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a68b8-188">Пример</span><span class="sxs-lookup"><span data-stu-id="a68b8-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="a68b8-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="a68b8-189">Request</span></span>
<span data-ttu-id="a68b8-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a68b8-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 429

{
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

### <a name="response"></a><span data-ttu-id="a68b8-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="a68b8-191">Response</span></span>
<span data-ttu-id="a68b8-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a68b8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





