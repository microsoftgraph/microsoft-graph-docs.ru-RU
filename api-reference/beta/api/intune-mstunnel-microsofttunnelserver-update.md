---
title: Обновление Микрософттуннелсервер
description: Обновление свойств объекта Микрософттуннелсервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5094f510552b8b27329b475e048141ba1165954
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301963"
---
# <a name="update-microsofttunnelserver"></a><span data-ttu-id="1cb64-103">Обновление Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="1cb64-103">Update microsoftTunnelServer</span></span>

<span data-ttu-id="1cb64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cb64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cb64-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cb64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cb64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cb64-107">Обновление свойств объекта [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) .</span><span class="sxs-lookup"><span data-stu-id="1cb64-107">Update the properties of a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cb64-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1cb64-108">Prerequisites</span></span>
<span data-ttu-id="1cb64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cb64-111">Permission type</span></span>|<span data-ttu-id="1cb64-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cb64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cb64-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cb64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cb64-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cb64-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cb64-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cb64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cb64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb64-116">Not supported.</span></span>|
|<span data-ttu-id="1cb64-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1cb64-117">Application</span></span>|<span data-ttu-id="1cb64-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cb64-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cb64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cb64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="request-headers"></a><span data-ttu-id="1cb64-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1cb64-120">Request headers</span></span>
|<span data-ttu-id="1cb64-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cb64-121">Header</span></span>|<span data-ttu-id="1cb64-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cb64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cb64-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cb64-123">Authorization</span></span>|<span data-ttu-id="1cb64-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cb64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cb64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cb64-125">Accept</span></span>|<span data-ttu-id="1cb64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cb64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cb64-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cb64-127">Request body</span></span>
<span data-ttu-id="1cb64-128">В тексте запроса добавьте представление объекта [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cb64-128">In the request body, supply a JSON representation for the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

<span data-ttu-id="1cb64-129">В следующей таблице приведены свойства, необходимые при создании [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md).</span><span class="sxs-lookup"><span data-stu-id="1cb64-129">The following table shows the properties that are required when you create the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).</span></span>

|<span data-ttu-id="1cb64-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cb64-130">Property</span></span>|<span data-ttu-id="1cb64-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb64-131">Type</span></span>|<span data-ttu-id="1cb64-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb64-133">id</span><span class="sxs-lookup"><span data-stu-id="1cb64-133">id</span></span>|<span data-ttu-id="1cb64-134">String</span><span class="sxs-lookup"><span data-stu-id="1cb64-134">String</span></span>|<span data-ttu-id="1cb64-135">Идентификатор Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="1cb64-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="1cb64-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1cb64-136">displayName</span></span>|<span data-ttu-id="1cb64-137">String</span><span class="sxs-lookup"><span data-stu-id="1cb64-137">String</span></span>|<span data-ttu-id="1cb64-138">Отображаемое имя Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="1cb64-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="1cb64-139">туннелсерверхеалсстатус</span><span class="sxs-lookup"><span data-stu-id="1cb64-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="1cb64-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="1cb64-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="1cb64-141">Состояние работоспособности Микрософттуннелсервер.</span><span class="sxs-lookup"><span data-stu-id="1cb64-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="1cb64-142">Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span><span class="sxs-lookup"><span data-stu-id="1cb64-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="1cb64-143">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="1cb64-143">lastCheckinDateTime</span></span>|<span data-ttu-id="1cb64-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cb64-144">DateTimeOffset</span></span>|<span data-ttu-id="1cb64-145">При последнем возвращенном Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="1cb64-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="1cb64-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cb64-146">Response</span></span>
<span data-ttu-id="1cb64-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1cb64-147">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb64-148">Пример</span><span class="sxs-lookup"><span data-stu-id="1cb64-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cb64-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cb64-149">Request</span></span>
<span data-ttu-id="1cb64-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cb64-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1cb64-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cb64-151">Response</span></span>
<span data-ttu-id="1cb64-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cb64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```




