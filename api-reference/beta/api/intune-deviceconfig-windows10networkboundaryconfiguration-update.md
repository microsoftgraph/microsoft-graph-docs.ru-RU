---
title: Обновление windows10NetworkBoundaryConfiguration
description: Обновление свойства объекта windows10NetworkBoundaryConfiguration.
ms.openlocfilehash: 3fb001ac9ad4c7538f9d201b8f3bf36f0d4f1f97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082179"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="d0fe0-103">Обновление windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fe0-103">Update windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="d0fe0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0fe0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0fe0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0fe0-107">Обновление свойства объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d0fe0-107">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0fe0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d0fe0-108">Prerequisites</span></span>
<span data-ttu-id="d0fe0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0fe0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0fe0-111">Permission type</span></span>|<span data-ttu-id="d0fe0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0fe0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0fe0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0fe0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0fe0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0fe0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0fe0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0fe0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0fe0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-116">Not supported.</span></span>|
|<span data-ttu-id="d0fe0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0fe0-117">Application</span></span>|<span data-ttu-id="d0fe0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0fe0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0fe0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d0fe0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0fe0-120">Request headers</span></span>
|<span data-ttu-id="d0fe0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0fe0-121">Header</span></span>|<span data-ttu-id="d0fe0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d0fe0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0fe0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0fe0-123">Authorization</span></span>|<span data-ttu-id="d0fe0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d0fe0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0fe0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0fe0-125">Accept</span></span>|<span data-ttu-id="d0fe0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0fe0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0fe0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0fe0-127">Request body</span></span>
<span data-ttu-id="d0fe0-128">В тексте запроса укажите представление JSON для объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d0fe0-128">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="d0fe0-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-129">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="d0fe0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0fe0-130">Property</span></span>|<span data-ttu-id="d0fe0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0fe0-131">Type</span></span>|<span data-ttu-id="d0fe0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0fe0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0fe0-133">id</span><span class="sxs-lookup"><span data-stu-id="d0fe0-133">id</span></span>|<span data-ttu-id="d0fe0-134">String</span><span class="sxs-lookup"><span data-stu-id="d0fe0-134">String</span></span>|<span data-ttu-id="d0fe0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-135">Key of the entity.</span></span> <span data-ttu-id="d0fe0-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fe0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d0fe0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fe0-138">DateTimeOffset</span></span>|<span data-ttu-id="d0fe0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d0fe0-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0fe0-141">roleScopeTagIds</span></span>|<span data-ttu-id="d0fe0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d0fe0-142">String collection</span></span>|<span data-ttu-id="d0fe0-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0fe0-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d0fe0-145">supportsScopeTags</span></span>|<span data-ttu-id="d0fe0-146">Логический</span><span class="sxs-lookup"><span data-stu-id="d0fe0-146">Boolean</span></span>|<span data-ttu-id="d0fe0-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0fe0-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0fe0-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0fe0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-150">This property is read-only.</span></span> <span data-ttu-id="d0fe0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fe0-152">createdDateTime</span></span>|<span data-ttu-id="d0fe0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fe0-153">DateTimeOffset</span></span>|<span data-ttu-id="d0fe0-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-154">DateTime the object was created.</span></span> <span data-ttu-id="d0fe0-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-156">описание</span><span class="sxs-lookup"><span data-stu-id="d0fe0-156">description</span></span>|<span data-ttu-id="d0fe0-157">String</span><span class="sxs-lookup"><span data-stu-id="d0fe0-157">String</span></span>|<span data-ttu-id="d0fe0-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0fe0-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d0fe0-160">displayName</span></span>|<span data-ttu-id="d0fe0-161">String</span><span class="sxs-lookup"><span data-stu-id="d0fe0-161">String</span></span>|<span data-ttu-id="d0fe0-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0fe0-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-164">version</span><span class="sxs-lookup"><span data-stu-id="d0fe0-164">version</span></span>|<span data-ttu-id="d0fe0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d0fe0-165">Int32</span></span>|<span data-ttu-id="d0fe0-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-166">Version of the device configuration.</span></span> <span data-ttu-id="d0fe0-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fe0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fe0-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="d0fe0-168">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="d0fe0-169">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="d0fe0-169">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="d0fe0-170">Политики изоляции сети Windows</span><span class="sxs-lookup"><span data-stu-id="d0fe0-170">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="d0fe0-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0fe0-171">Response</span></span>
<span data-ttu-id="d0fe0-172">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-172">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0fe0-173">Пример</span><span class="sxs-lookup"><span data-stu-id="d0fe0-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0fe0-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0fe0-174">Request</span></span>
<span data-ttu-id="d0fe0-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0fe0-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1232

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d0fe0-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0fe0-176">Response</span></span>
<span data-ttu-id="d0fe0-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d0fe0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





