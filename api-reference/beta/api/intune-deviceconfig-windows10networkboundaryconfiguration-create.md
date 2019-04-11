---
title: Создание windows10NetworkBoundaryConfiguration
description: Создание нового объекта windows10NetworkBoundaryConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a85fcb44c022266b1f920664083a2ffe6a997cc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780632"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="f1790-103">Создание windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1790-103">Create windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="f1790-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1790-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1790-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1790-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1790-106">Создание нового объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1790-106">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1790-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1790-107">Prerequisites</span></span>
<span data-ttu-id="f1790-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1790-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1790-110">Permission type</span></span>|<span data-ttu-id="f1790-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1790-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1790-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1790-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1790-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1790-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1790-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1790-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1790-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1790-115">Not supported.</span></span>|
|<span data-ttu-id="f1790-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1790-116">Application</span></span>|<span data-ttu-id="f1790-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1790-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1790-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1790-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f1790-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1790-119">Request headers</span></span>
|<span data-ttu-id="f1790-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1790-120">Header</span></span>|<span data-ttu-id="f1790-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f1790-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1790-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1790-122">Authorization</span></span>|<span data-ttu-id="f1790-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1790-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1790-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f1790-124">Accept</span></span>|<span data-ttu-id="f1790-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1790-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1790-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1790-126">Request body</span></span>
<span data-ttu-id="f1790-127">В тексте запроса добавьте представление объекта windows10NetworkBoundaryConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1790-127">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="f1790-128">В следующей таблице приведены свойства, необходимые при создании windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1790-128">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="f1790-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1790-129">Property</span></span>|<span data-ttu-id="f1790-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f1790-130">Type</span></span>|<span data-ttu-id="f1790-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f1790-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1790-132">id</span><span class="sxs-lookup"><span data-stu-id="f1790-132">id</span></span>|<span data-ttu-id="f1790-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f1790-133">String</span></span>|<span data-ttu-id="f1790-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1790-134">Key of the entity.</span></span> <span data-ttu-id="f1790-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1790-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f1790-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1790-137">DateTimeOffset</span></span>|<span data-ttu-id="f1790-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f1790-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f1790-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1790-140">roleScopeTagIds</span></span>|<span data-ttu-id="f1790-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1790-141">String collection</span></span>|<span data-ttu-id="f1790-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f1790-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1790-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f1790-144">supportsScopeTags</span></span>|<span data-ttu-id="f1790-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1790-145">Boolean</span></span>|<span data-ttu-id="f1790-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f1790-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1790-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f1790-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1790-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f1790-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1790-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1790-149">This property is read-only.</span></span> <span data-ttu-id="f1790-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1790-151">createdDateTime</span></span>|<span data-ttu-id="f1790-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1790-152">DateTimeOffset</span></span>|<span data-ttu-id="f1790-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f1790-153">DateTime the object was created.</span></span> <span data-ttu-id="f1790-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-155">description</span><span class="sxs-lookup"><span data-stu-id="f1790-155">description</span></span>|<span data-ttu-id="f1790-156">String</span><span class="sxs-lookup"><span data-stu-id="f1790-156">String</span></span>|<span data-ttu-id="f1790-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1790-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1790-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f1790-159">displayName</span></span>|<span data-ttu-id="f1790-160">String</span><span class="sxs-lookup"><span data-stu-id="f1790-160">String</span></span>|<span data-ttu-id="f1790-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1790-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1790-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-163">version</span><span class="sxs-lookup"><span data-stu-id="f1790-163">version</span></span>|<span data-ttu-id="f1790-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f1790-164">Int32</span></span>|<span data-ttu-id="f1790-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1790-165">Version of the device configuration.</span></span> <span data-ttu-id="f1790-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1790-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1790-167">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="f1790-167">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="f1790-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="f1790-168">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="f1790-169">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="f1790-169">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="f1790-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1790-170">Response</span></span>
<span data-ttu-id="f1790-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1790-171">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1790-172">Пример</span><span class="sxs-lookup"><span data-stu-id="f1790-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1790-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1790-173">Request</span></span>
<span data-ttu-id="f1790-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1790-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f1790-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1790-175">Response</span></span>
<span data-ttu-id="f1790-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1790-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





