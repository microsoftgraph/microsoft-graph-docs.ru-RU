---
title: Обновление windows10NetworkBoundaryConfiguration
description: Обновление свойств объекта windows10NetworkBoundaryConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d9a5e8c5cd8e0d4566f99897e059710f58669c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145257"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="a3d81-103">Обновление windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3d81-103">Update windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="a3d81-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3d81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3d81-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3d81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3d81-106">Обновление свойств объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a3d81-106">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3d81-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3d81-107">Prerequisites</span></span>
<span data-ttu-id="a3d81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3d81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3d81-110">Permission type</span></span>|<span data-ttu-id="a3d81-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3d81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3d81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3d81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3d81-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d81-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3d81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3d81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3d81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3d81-115">Not supported.</span></span>|
|<span data-ttu-id="a3d81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3d81-116">Application</span></span>|<span data-ttu-id="a3d81-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3d81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3d81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3d81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a3d81-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3d81-119">Request headers</span></span>
|<span data-ttu-id="a3d81-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3d81-120">Header</span></span>|<span data-ttu-id="a3d81-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3d81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3d81-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3d81-122">Authorization</span></span>|<span data-ttu-id="a3d81-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3d81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3d81-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3d81-124">Accept</span></span>|<span data-ttu-id="a3d81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3d81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3d81-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3d81-126">Request body</span></span>
<span data-ttu-id="a3d81-127">В тексте запроса добавьте представление объекта [Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3d81-127">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="a3d81-128">В следующей таблице приведены свойства, необходимые при создании [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-128">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="a3d81-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3d81-129">Property</span></span>|<span data-ttu-id="a3d81-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a3d81-130">Type</span></span>|<span data-ttu-id="a3d81-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a3d81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3d81-132">id</span><span class="sxs-lookup"><span data-stu-id="a3d81-132">id</span></span>|<span data-ttu-id="a3d81-133">String</span><span class="sxs-lookup"><span data-stu-id="a3d81-133">String</span></span>|<span data-ttu-id="a3d81-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3d81-134">Key of the entity.</span></span> <span data-ttu-id="a3d81-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3d81-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a3d81-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3d81-137">DateTimeOffset</span></span>|<span data-ttu-id="a3d81-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a3d81-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a3d81-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3d81-140">roleScopeTagIds</span></span>|<span data-ttu-id="a3d81-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a3d81-141">String collection</span></span>|<span data-ttu-id="a3d81-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a3d81-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a3d81-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a3d81-144">supportsScopeTags</span></span>|<span data-ttu-id="a3d81-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a3d81-145">Boolean</span></span>|<span data-ttu-id="a3d81-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a3d81-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a3d81-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a3d81-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a3d81-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a3d81-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a3d81-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3d81-149">This property is read-only.</span></span> <span data-ttu-id="a3d81-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3d81-151">createdDateTime</span></span>|<span data-ttu-id="a3d81-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3d81-152">DateTimeOffset</span></span>|<span data-ttu-id="a3d81-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a3d81-153">DateTime the object was created.</span></span> <span data-ttu-id="a3d81-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-155">description</span><span class="sxs-lookup"><span data-stu-id="a3d81-155">description</span></span>|<span data-ttu-id="a3d81-156">String</span><span class="sxs-lookup"><span data-stu-id="a3d81-156">String</span></span>|<span data-ttu-id="a3d81-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3d81-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3d81-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a3d81-159">displayName</span></span>|<span data-ttu-id="a3d81-160">String</span><span class="sxs-lookup"><span data-stu-id="a3d81-160">String</span></span>|<span data-ttu-id="a3d81-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3d81-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3d81-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-163">version</span><span class="sxs-lookup"><span data-stu-id="a3d81-163">version</span></span>|<span data-ttu-id="a3d81-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d81-164">Int32</span></span>|<span data-ttu-id="a3d81-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3d81-165">Version of the device configuration.</span></span> <span data-ttu-id="a3d81-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3d81-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3d81-167">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="a3d81-167">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="a3d81-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="a3d81-168">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="a3d81-169">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="a3d81-169">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="a3d81-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3d81-170">Response</span></span>
<span data-ttu-id="a3d81-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3d81-171">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3d81-172">Пример</span><span class="sxs-lookup"><span data-stu-id="a3d81-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3d81-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3d81-173">Request</span></span>
<span data-ttu-id="a3d81-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3d81-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="a3d81-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3d81-175">Response</span></span>
<span data-ttu-id="a3d81-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3d81-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```




