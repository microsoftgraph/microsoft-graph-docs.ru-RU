---
title: Обновление объекта editionUpgradeConfiguration
description: Обновление свойств объекта editionUpgradeConfiguration.
author: tfitzmac
ms.openlocfilehash: 2ece07f1d0efbcf67f4c28a8fcc3dd2a0b349287
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302116"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="c92e7-103">Обновление объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c92e7-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="c92e7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c92e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c92e7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c92e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c92e7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c92e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c92e7-107">Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c92e7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c92e7-108">Prerequisites</span></span>
<span data-ttu-id="c92e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c92e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c92e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c92e7-111">Permission type</span></span>|<span data-ttu-id="c92e7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c92e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c92e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c92e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c92e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c92e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c92e7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c92e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c92e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c92e7-116">Not supported.</span></span>|
|<span data-ttu-id="c92e7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c92e7-117">Application</span></span>|<span data-ttu-id="c92e7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c92e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c92e7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c92e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c92e7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c92e7-120">Request headers</span></span>
|<span data-ttu-id="c92e7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c92e7-121">Header</span></span>|<span data-ttu-id="c92e7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c92e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c92e7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c92e7-123">Authorization</span></span>|<span data-ttu-id="c92e7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c92e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c92e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c92e7-125">Accept</span></span>|<span data-ttu-id="c92e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c92e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c92e7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c92e7-127">Request body</span></span>
<span data-ttu-id="c92e7-128">В теле запроса добавьте представление объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c92e7-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="c92e7-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="c92e7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c92e7-130">Property</span></span>|<span data-ttu-id="c92e7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c92e7-131">Type</span></span>|<span data-ttu-id="c92e7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c92e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c92e7-133">id</span><span class="sxs-lookup"><span data-stu-id="c92e7-133">id</span></span>|<span data-ttu-id="c92e7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c92e7-134">String</span></span>|<span data-ttu-id="c92e7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c92e7-135">Key of the entity.</span></span> <span data-ttu-id="c92e7-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c92e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c92e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c92e7-138">DateTimeOffset</span></span>|<span data-ttu-id="c92e7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c92e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c92e7-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c92e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="c92e7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c92e7-142">String collection</span></span>|<span data-ttu-id="c92e7-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c92e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c92e7-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c92e7-145">supportsScopeTags</span></span>|<span data-ttu-id="c92e7-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c92e7-146">Boolean</span></span>|<span data-ttu-id="c92e7-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c92e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c92e7-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c92e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c92e7-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c92e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c92e7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c92e7-150">This property is read-only.</span></span> <span data-ttu-id="c92e7-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c92e7-152">createdDateTime</span></span>|<span data-ttu-id="c92e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c92e7-153">DateTimeOffset</span></span>|<span data-ttu-id="c92e7-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c92e7-154">DateTime the object was created.</span></span> <span data-ttu-id="c92e7-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-156">описание</span><span class="sxs-lookup"><span data-stu-id="c92e7-156">description</span></span>|<span data-ttu-id="c92e7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c92e7-157">String</span></span>|<span data-ttu-id="c92e7-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c92e7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c92e7-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c92e7-160">displayName</span></span>|<span data-ttu-id="c92e7-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c92e7-161">String</span></span>|<span data-ttu-id="c92e7-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c92e7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c92e7-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-164">version</span><span class="sxs-lookup"><span data-stu-id="c92e7-164">version</span></span>|<span data-ttu-id="c92e7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c92e7-165">Int32</span></span>|<span data-ttu-id="c92e7-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c92e7-166">Version of the device configuration.</span></span> <span data-ttu-id="c92e7-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c92e7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c92e7-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="c92e7-168">licenseType</span></span>|[<span data-ttu-id="c92e7-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="c92e7-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="c92e7-170">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="c92e7-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="c92e7-171">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="c92e7-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="c92e7-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="c92e7-172">targetEdition</span></span>|[<span data-ttu-id="c92e7-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="c92e7-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="c92e7-174">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="c92e7-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="c92e7-175">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="c92e7-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="c92e7-176">license</span><span class="sxs-lookup"><span data-stu-id="c92e7-176">license</span></span>|<span data-ttu-id="c92e7-177">String</span><span class="sxs-lookup"><span data-stu-id="c92e7-177">String</span></span>|<span data-ttu-id="c92e7-178">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="c92e7-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="c92e7-179">productKey</span><span class="sxs-lookup"><span data-stu-id="c92e7-179">productKey</span></span>|<span data-ttu-id="c92e7-180">String</span><span class="sxs-lookup"><span data-stu-id="c92e7-180">String</span></span>|<span data-ttu-id="c92e7-181">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="c92e7-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="c92e7-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="c92e7-182">windowsSMode</span></span>|[<span data-ttu-id="c92e7-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c92e7-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="c92e7-184">Конфигурация S.</span><span class="sxs-lookup"><span data-stu-id="c92e7-184">S mode configuration.</span></span> <span data-ttu-id="c92e7-185">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="c92e7-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="c92e7-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="c92e7-186">Response</span></span>
<span data-ttu-id="c92e7-187">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c92e7-187">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c92e7-188">Пример</span><span class="sxs-lookup"><span data-stu-id="c92e7-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="c92e7-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="c92e7-189">Request</span></span>
<span data-ttu-id="c92e7-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c92e7-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c92e7-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="c92e7-191">Response</span></span>
<span data-ttu-id="c92e7-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c92e7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





