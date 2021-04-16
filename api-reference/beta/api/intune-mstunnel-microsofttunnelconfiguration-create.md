---
title: Создание microsoftTunnelConfiguration
description: Создайте новый объект microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e17cd32c6fedf529cab0c840bea93e7d81c1a4cf
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868157"
---
# <a name="create-microsofttunnelconfiguration"></a><span data-ttu-id="2e1ba-103">Создание microsoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e1ba-103">Create microsoftTunnelConfiguration</span></span>

<span data-ttu-id="2e1ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e1ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e1ba-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e1ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e1ba-107">Создайте [новый объект microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2e1ba-107">Create a new [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e1ba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e1ba-108">Prerequisites</span></span>
<span data-ttu-id="2e1ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e1ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e1ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e1ba-111">Permission type</span></span>|<span data-ttu-id="2e1ba-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e1ba-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e1ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e1ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e1ba-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e1ba-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="2e1ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e1ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e1ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-116">Not supported.</span></span>|
|<span data-ttu-id="2e1ba-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2e1ba-117">Application</span></span>|<span data-ttu-id="2e1ba-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e1ba-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e1ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e1ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2e1ba-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e1ba-120">Request headers</span></span>
|<span data-ttu-id="2e1ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e1ba-121">Header</span></span>|<span data-ttu-id="2e1ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e1ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e1ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e1ba-123">Authorization</span></span>|<span data-ttu-id="2e1ba-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e1ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e1ba-125">Accept</span></span>|<span data-ttu-id="2e1ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e1ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e1ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e1ba-127">Request body</span></span>
<span data-ttu-id="2e1ba-128">В теле запроса предоставляем представление JSON для объекта MicrosoftTunnelConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-128">In the request body, supply a JSON representation for the microsoftTunnelConfiguration object.</span></span>

<span data-ttu-id="2e1ba-129">В следующей таблице показаны свойства, необходимые при создании microsoftTunnelConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-129">The following table shows the properties that are required when you create the microsoftTunnelConfiguration.</span></span>

|<span data-ttu-id="2e1ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e1ba-130">Property</span></span>|<span data-ttu-id="2e1ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2e1ba-131">Type</span></span>|<span data-ttu-id="2e1ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2e1ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e1ba-133">id</span><span class="sxs-lookup"><span data-stu-id="2e1ba-133">id</span></span>|<span data-ttu-id="2e1ba-134">String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-134">String</span></span>|<span data-ttu-id="2e1ba-135">Id MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e1ba-135">The MicrosoftTunnelConfiguration's Id</span></span>|
|<span data-ttu-id="2e1ba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e1ba-136">displayName</span></span>|<span data-ttu-id="2e1ba-137">String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-137">String</span></span>|<span data-ttu-id="2e1ba-138">Имя отображения MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e1ba-138">The MicrosoftTunnelConfiguration's display name</span></span>|
|<span data-ttu-id="2e1ba-139">description</span><span class="sxs-lookup"><span data-stu-id="2e1ba-139">description</span></span>|<span data-ttu-id="2e1ba-140">String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-140">String</span></span>|<span data-ttu-id="2e1ba-141">Описание MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e1ba-141">The MicrosoftTunnelConfiguration's description</span></span>|
|<span data-ttu-id="2e1ba-142">сеть</span><span class="sxs-lookup"><span data-stu-id="2e1ba-142">network</span></span>|<span data-ttu-id="2e1ba-143">String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-143">String</span></span>|<span data-ttu-id="2e1ba-144">Подсеть, которая будет использоваться для выделения виртуального адреса для клиентов</span><span class="sxs-lookup"><span data-stu-id="2e1ba-144">The subnet that will be used to allocate virtual address for the clients</span></span>|
|<span data-ttu-id="2e1ba-145">dnsServers</span><span class="sxs-lookup"><span data-stu-id="2e1ba-145">dnsServers</span></span>|<span data-ttu-id="2e1ba-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-146">String collection</span></span>|<span data-ttu-id="2e1ba-147">DNS-серверы, которые будут использоваться клиентами</span><span class="sxs-lookup"><span data-stu-id="2e1ba-147">The DNS servers that will be used by the clients</span></span>|
|<span data-ttu-id="2e1ba-148">defaultDomainSuffix</span><span class="sxs-lookup"><span data-stu-id="2e1ba-148">defaultDomainSuffix</span></span>|<span data-ttu-id="2e1ba-149">String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-149">String</span></span>|<span data-ttu-id="2e1ba-150">Приложение домена по умолчанию, которое будет использоваться клиентами</span><span class="sxs-lookup"><span data-stu-id="2e1ba-150">The Default Domain appendix that will be used by the clients</span></span>|
|<span data-ttu-id="2e1ba-151">routesInclude</span><span class="sxs-lookup"><span data-stu-id="2e1ba-151">routesInclude</span></span>|<span data-ttu-id="2e1ba-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-152">String collection</span></span>|<span data-ttu-id="2e1ba-153">Маршруты, которые будут маршрутить сервер</span><span class="sxs-lookup"><span data-stu-id="2e1ba-153">The routs that will be routed by the server</span></span>|
|<span data-ttu-id="2e1ba-154">routesExclude</span><span class="sxs-lookup"><span data-stu-id="2e1ba-154">routesExclude</span></span>|<span data-ttu-id="2e1ba-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-155">String collection</span></span>|<span data-ttu-id="2e1ba-156">Подмышы маршрутов, которые не будут маршрутиться сервером</span><span class="sxs-lookup"><span data-stu-id="2e1ba-156">Subsets of the routes that will not be routed by the server</span></span>|
|<span data-ttu-id="2e1ba-157">splitDNS</span><span class="sxs-lookup"><span data-stu-id="2e1ba-157">splitDNS</span></span>|<span data-ttu-id="2e1ba-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-158">String collection</span></span>|<span data-ttu-id="2e1ba-159">Домены, которые будут разрешены с помощью предоставленных dns-серверов</span><span class="sxs-lookup"><span data-stu-id="2e1ba-159">The domains that will be resolved using the provided dns servers</span></span>|
|<span data-ttu-id="2e1ba-160">listenPort</span><span class="sxs-lookup"><span data-stu-id="2e1ba-160">listenPort</span></span>|<span data-ttu-id="2e1ba-161">Int32</span><span class="sxs-lookup"><span data-stu-id="2e1ba-161">Int32</span></span>|<span data-ttu-id="2e1ba-162">Порт, который будут прослушивать TCP и UPD на сервере</span><span class="sxs-lookup"><span data-stu-id="2e1ba-162">The port that both TCP and UPD will listen over on the server</span></span>|
|<span data-ttu-id="2e1ba-163">advancedSettings</span><span class="sxs-lookup"><span data-stu-id="2e1ba-163">advancedSettings</span></span>|<span data-ttu-id="2e1ba-164">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2e1ba-164">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2e1ba-165">Дополнительные параметры, которые могут быть применены к серверу</span><span class="sxs-lookup"><span data-stu-id="2e1ba-165">Additional settings that may be applied to the server</span></span>|
|<span data-ttu-id="2e1ba-166">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2e1ba-166">lastUpdateDateTime</span></span>|<span data-ttu-id="2e1ba-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e1ba-167">DateTimeOffset</span></span>|<span data-ttu-id="2e1ba-168">При последнем обновлении MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e1ba-168">When the MicrosoftTunnelConfiguration was last updated</span></span>|
|<span data-ttu-id="2e1ba-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2e1ba-169">roleScopeTagIds</span></span>|<span data-ttu-id="2e1ba-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e1ba-170">String collection</span></span>|<span data-ttu-id="2e1ba-171">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2e1ba-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e1ba-172">Response</span></span>
<span data-ttu-id="2e1ba-173">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-173">If successful, this method returns a `201 Created` response code and a [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e1ba-174">Пример</span><span class="sxs-lookup"><span data-stu-id="2e1ba-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e1ba-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e1ba-175">Request</span></span>
<span data-ttu-id="2e1ba-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e1ba-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e1ba-177">Response</span></span>
<span data-ttu-id="2e1ba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e1ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




