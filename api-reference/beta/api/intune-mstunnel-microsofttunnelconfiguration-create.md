---
title: Создание Микрософттуннелконфигуратион
description: Создание нового объекта Микрософттуннелконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa74bc55c739cc7ef8ad735538e9a948cfc2a2a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242352"
---
# <a name="create-microsofttunnelconfiguration"></a><span data-ttu-id="571fd-103">Создание Микрософттуннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="571fd-103">Create microsoftTunnelConfiguration</span></span>

<span data-ttu-id="571fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="571fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="571fd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="571fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="571fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="571fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="571fd-107">Создание нового объекта [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="571fd-107">Create a new [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="571fd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="571fd-108">Prerequisites</span></span>
<span data-ttu-id="571fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="571fd-111">Permission type</span></span>|<span data-ttu-id="571fd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="571fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="571fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="571fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="571fd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="571fd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="571fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="571fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="571fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="571fd-116">Not supported.</span></span>|
|<span data-ttu-id="571fd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="571fd-117">Application</span></span>|<span data-ttu-id="571fd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="571fd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="571fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="571fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="571fd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="571fd-120">Request headers</span></span>
|<span data-ttu-id="571fd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="571fd-121">Header</span></span>|<span data-ttu-id="571fd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="571fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="571fd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="571fd-123">Authorization</span></span>|<span data-ttu-id="571fd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="571fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="571fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="571fd-125">Accept</span></span>|<span data-ttu-id="571fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="571fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="571fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="571fd-127">Request body</span></span>
<span data-ttu-id="571fd-128">В тексте запроса добавьте представление объекта Микрософттуннелконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="571fd-128">In the request body, supply a JSON representation for the microsoftTunnelConfiguration object.</span></span>

<span data-ttu-id="571fd-129">В следующей таблице приведены свойства, необходимые при создании Микрософттуннелконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="571fd-129">The following table shows the properties that are required when you create the microsoftTunnelConfiguration.</span></span>

|<span data-ttu-id="571fd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="571fd-130">Property</span></span>|<span data-ttu-id="571fd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="571fd-131">Type</span></span>|<span data-ttu-id="571fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="571fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="571fd-133">id</span><span class="sxs-lookup"><span data-stu-id="571fd-133">id</span></span>|<span data-ttu-id="571fd-134">String</span><span class="sxs-lookup"><span data-stu-id="571fd-134">String</span></span>|<span data-ttu-id="571fd-135">Идентификатор Микрософттуннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="571fd-135">The MicrosoftTunnelConfiguration's Id</span></span>|
|<span data-ttu-id="571fd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="571fd-136">displayName</span></span>|<span data-ttu-id="571fd-137">String</span><span class="sxs-lookup"><span data-stu-id="571fd-137">String</span></span>|<span data-ttu-id="571fd-138">Отображаемое имя Микрософттуннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="571fd-138">The MicrosoftTunnelConfiguration's display name</span></span>|
|<span data-ttu-id="571fd-139">description</span><span class="sxs-lookup"><span data-stu-id="571fd-139">description</span></span>|<span data-ttu-id="571fd-140">String</span><span class="sxs-lookup"><span data-stu-id="571fd-140">String</span></span>|<span data-ttu-id="571fd-141">Описание Микрософттуннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="571fd-141">The MicrosoftTunnelConfiguration's description</span></span>|
|<span data-ttu-id="571fd-142">сетью</span><span class="sxs-lookup"><span data-stu-id="571fd-142">network</span></span>|<span data-ttu-id="571fd-143">String</span><span class="sxs-lookup"><span data-stu-id="571fd-143">String</span></span>|<span data-ttu-id="571fd-144">Подсеть, которая будет использоваться для выделения виртуального адреса для клиентов.</span><span class="sxs-lookup"><span data-stu-id="571fd-144">The subnet that will be used to allocate virtual address for the clients</span></span>|
|<span data-ttu-id="571fd-145">днссерверс</span><span class="sxs-lookup"><span data-stu-id="571fd-145">dnsServers</span></span>|<span data-ttu-id="571fd-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="571fd-146">String collection</span></span>|<span data-ttu-id="571fd-147">DNS-серверы, которые будут использоваться клиентами;</span><span class="sxs-lookup"><span data-stu-id="571fd-147">The DNS servers that will be used by the clients</span></span>|
|<span data-ttu-id="571fd-148">дефаултдомаинсуффикс</span><span class="sxs-lookup"><span data-stu-id="571fd-148">defaultDomainSuffix</span></span>|<span data-ttu-id="571fd-149">String</span><span class="sxs-lookup"><span data-stu-id="571fd-149">String</span></span>|<span data-ttu-id="571fd-150">Приложение домена по умолчанию, которое будет использоваться клиентами.</span><span class="sxs-lookup"><span data-stu-id="571fd-150">The Default Domain appendix that will be used by the clients</span></span>|
|<span data-ttu-id="571fd-151">раутесинклуде</span><span class="sxs-lookup"><span data-stu-id="571fd-151">routesInclude</span></span>|<span data-ttu-id="571fd-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="571fd-152">String collection</span></span>|<span data-ttu-id="571fd-153">Маршрутизации, которые будут маршрутизироваться сервером</span><span class="sxs-lookup"><span data-stu-id="571fd-153">The routs that will be routed by the server</span></span>|
|<span data-ttu-id="571fd-154">раутесексклуде</span><span class="sxs-lookup"><span data-stu-id="571fd-154">routesExclude</span></span>|<span data-ttu-id="571fd-155">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="571fd-155">String collection</span></span>|<span data-ttu-id="571fd-156">Подмножества маршрутов, которые не будут маршрутизироваться сервером</span><span class="sxs-lookup"><span data-stu-id="571fd-156">Subsets of the routes that will not be routed by the server</span></span>|
|<span data-ttu-id="571fd-157">сплитднс</span><span class="sxs-lookup"><span data-stu-id="571fd-157">splitDNS</span></span>|<span data-ttu-id="571fd-158">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="571fd-158">String collection</span></span>|<span data-ttu-id="571fd-159">Домены, которые будут разрешены с помощью предоставленных DNS-серверов</span><span class="sxs-lookup"><span data-stu-id="571fd-159">The domains that will be resolved using the provided dns servers</span></span>|
|<span data-ttu-id="571fd-160">листенпорт</span><span class="sxs-lookup"><span data-stu-id="571fd-160">listenPort</span></span>|<span data-ttu-id="571fd-161">Int32</span><span class="sxs-lookup"><span data-stu-id="571fd-161">Int32</span></span>|<span data-ttu-id="571fd-162">Порт, прослушиваемый портами TCP и UPD на сервере</span><span class="sxs-lookup"><span data-stu-id="571fd-162">The port that both TCP and UPD will listen over on the server</span></span>|
|<span data-ttu-id="571fd-163">адванцедсеттингс</span><span class="sxs-lookup"><span data-stu-id="571fd-163">advancedSettings</span></span>|<span data-ttu-id="571fd-164">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="571fd-164">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="571fd-165">Дополнительные параметры, которые могут быть применены к серверу</span><span class="sxs-lookup"><span data-stu-id="571fd-165">Additional settings that may be applied to the server</span></span>|
|<span data-ttu-id="571fd-166">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="571fd-166">lastUpdateDateTime</span></span>|<span data-ttu-id="571fd-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="571fd-167">DateTimeOffset</span></span>|<span data-ttu-id="571fd-168">При последнем обновлении Микрософттуннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="571fd-168">When the MicrosoftTunnelConfiguration was last updated</span></span>|
|<span data-ttu-id="571fd-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="571fd-169">roleScopeTagIds</span></span>|<span data-ttu-id="571fd-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="571fd-170">String collection</span></span>|<span data-ttu-id="571fd-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="571fd-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="571fd-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="571fd-172">Response</span></span>
<span data-ttu-id="571fd-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="571fd-173">If successful, this method returns a `201 Created` response code and a [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571fd-174">Пример</span><span class="sxs-lookup"><span data-stu-id="571fd-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="571fd-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="571fd-175">Request</span></span>
<span data-ttu-id="571fd-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="571fd-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="571fd-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="571fd-177">Response</span></span>
<span data-ttu-id="571fd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="571fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 797

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




