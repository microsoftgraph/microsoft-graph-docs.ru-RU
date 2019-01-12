---
title: Обновление windows10NetworkBoundaryConfiguration
description: Обновление свойства объекта windows10NetworkBoundaryConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d9b5e58987e20a922e67b412de74313c7a7ac47a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939716"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="fb56c-103">Обновление windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb56c-103">Update windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="fb56c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb56c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb56c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb56c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb56c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb56c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb56c-107">Обновление свойства объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fb56c-107">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb56c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb56c-108">Prerequisites</span></span>
<span data-ttu-id="fb56c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb56c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb56c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb56c-111">Permission type</span></span>|<span data-ttu-id="fb56c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb56c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb56c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb56c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb56c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb56c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb56c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb56c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb56c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb56c-116">Not supported.</span></span>|
|<span data-ttu-id="fb56c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb56c-117">Application</span></span>|<span data-ttu-id="fb56c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb56c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb56c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb56c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fb56c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb56c-120">Request headers</span></span>
|<span data-ttu-id="fb56c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb56c-121">Header</span></span>|<span data-ttu-id="fb56c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb56c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb56c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb56c-123">Authorization</span></span>|<span data-ttu-id="fb56c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb56c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb56c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb56c-125">Accept</span></span>|<span data-ttu-id="fb56c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb56c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb56c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb56c-127">Request body</span></span>
<span data-ttu-id="fb56c-128">В тексте запроса укажите представление JSON для объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fb56c-128">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="fb56c-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-129">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="fb56c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb56c-130">Property</span></span>|<span data-ttu-id="fb56c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb56c-131">Type</span></span>|<span data-ttu-id="fb56c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb56c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb56c-133">id</span><span class="sxs-lookup"><span data-stu-id="fb56c-133">id</span></span>|<span data-ttu-id="fb56c-134">String</span><span class="sxs-lookup"><span data-stu-id="fb56c-134">String</span></span>|<span data-ttu-id="fb56c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb56c-135">Key of the entity.</span></span> <span data-ttu-id="fb56c-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb56c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fb56c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb56c-138">DateTimeOffset</span></span>|<span data-ttu-id="fb56c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb56c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fb56c-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb56c-141">roleScopeTagIds</span></span>|<span data-ttu-id="fb56c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb56c-142">String collection</span></span>|<span data-ttu-id="fb56c-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fb56c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fb56c-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fb56c-145">supportsScopeTags</span></span>|<span data-ttu-id="fb56c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb56c-146">Boolean</span></span>|<span data-ttu-id="fb56c-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fb56c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fb56c-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fb56c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fb56c-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fb56c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fb56c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb56c-150">This property is read-only.</span></span> <span data-ttu-id="fb56c-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb56c-152">createdDateTime</span></span>|<span data-ttu-id="fb56c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb56c-153">DateTimeOffset</span></span>|<span data-ttu-id="fb56c-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb56c-154">DateTime the object was created.</span></span> <span data-ttu-id="fb56c-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-156">описание</span><span class="sxs-lookup"><span data-stu-id="fb56c-156">description</span></span>|<span data-ttu-id="fb56c-157">String</span><span class="sxs-lookup"><span data-stu-id="fb56c-157">String</span></span>|<span data-ttu-id="fb56c-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb56c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb56c-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fb56c-160">displayName</span></span>|<span data-ttu-id="fb56c-161">String</span><span class="sxs-lookup"><span data-stu-id="fb56c-161">String</span></span>|<span data-ttu-id="fb56c-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb56c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb56c-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-164">version</span><span class="sxs-lookup"><span data-stu-id="fb56c-164">version</span></span>|<span data-ttu-id="fb56c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fb56c-165">Int32</span></span>|<span data-ttu-id="fb56c-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb56c-166">Version of the device configuration.</span></span> <span data-ttu-id="fb56c-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb56c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb56c-168">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="fb56c-168">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="fb56c-169">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="fb56c-169">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="fb56c-170">Политики изоляции сети Windows</span><span class="sxs-lookup"><span data-stu-id="fb56c-170">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="fb56c-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb56c-171">Response</span></span>
<span data-ttu-id="fb56c-172">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb56c-172">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb56c-173">Пример</span><span class="sxs-lookup"><span data-stu-id="fb56c-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb56c-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb56c-174">Request</span></span>
<span data-ttu-id="fb56c-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb56c-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb56c-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb56c-176">Response</span></span>
<span data-ttu-id="fb56c-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb56c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





