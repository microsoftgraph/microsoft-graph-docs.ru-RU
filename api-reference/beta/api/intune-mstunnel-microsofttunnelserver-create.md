---
title: Создание Микрософттуннелсервер
description: Создание нового объекта Микрософттуннелсервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146de9c8b03d2934ad6507b5adf2aecc3d778d75
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301984"
---
# <a name="create-microsofttunnelserver"></a><span data-ttu-id="f86e1-103">Создание Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="f86e1-103">Create microsoftTunnelServer</span></span>

<span data-ttu-id="f86e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f86e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f86e1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f86e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f86e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f86e1-107">Создание нового объекта [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) .</span><span class="sxs-lookup"><span data-stu-id="f86e1-107">Create a new [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f86e1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f86e1-108">Prerequisites</span></span>
<span data-ttu-id="f86e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f86e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f86e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f86e1-111">Permission type</span></span>|<span data-ttu-id="f86e1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f86e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f86e1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f86e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f86e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f86e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f86e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f86e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f86e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86e1-116">Not supported.</span></span>|
|<span data-ttu-id="f86e1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f86e1-117">Application</span></span>|<span data-ttu-id="f86e1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f86e1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f86e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f86e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a><span data-ttu-id="f86e1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f86e1-120">Request headers</span></span>
|<span data-ttu-id="f86e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f86e1-121">Header</span></span>|<span data-ttu-id="f86e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f86e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f86e1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f86e1-123">Authorization</span></span>|<span data-ttu-id="f86e1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f86e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f86e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f86e1-125">Accept</span></span>|<span data-ttu-id="f86e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f86e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f86e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f86e1-127">Request body</span></span>
<span data-ttu-id="f86e1-128">В тексте запроса добавьте представление объекта Микрософттуннелсервер в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f86e1-128">In the request body, supply a JSON representation for the microsoftTunnelServer object.</span></span>

<span data-ttu-id="f86e1-129">В следующей таблице приведены свойства, необходимые при создании Микрософттуннелсервер.</span><span class="sxs-lookup"><span data-stu-id="f86e1-129">The following table shows the properties that are required when you create the microsoftTunnelServer.</span></span>

|<span data-ttu-id="f86e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f86e1-130">Property</span></span>|<span data-ttu-id="f86e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f86e1-131">Type</span></span>|<span data-ttu-id="f86e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f86e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f86e1-133">id</span><span class="sxs-lookup"><span data-stu-id="f86e1-133">id</span></span>|<span data-ttu-id="f86e1-134">String</span><span class="sxs-lookup"><span data-stu-id="f86e1-134">String</span></span>|<span data-ttu-id="f86e1-135">Идентификатор Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="f86e1-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="f86e1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f86e1-136">displayName</span></span>|<span data-ttu-id="f86e1-137">String</span><span class="sxs-lookup"><span data-stu-id="f86e1-137">String</span></span>|<span data-ttu-id="f86e1-138">Отображаемое имя Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="f86e1-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="f86e1-139">туннелсерверхеалсстатус</span><span class="sxs-lookup"><span data-stu-id="f86e1-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="f86e1-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="f86e1-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="f86e1-141">Состояние работоспособности Микрософттуннелсервер.</span><span class="sxs-lookup"><span data-stu-id="f86e1-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="f86e1-142">Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span><span class="sxs-lookup"><span data-stu-id="f86e1-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="f86e1-143">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="f86e1-143">lastCheckinDateTime</span></span>|<span data-ttu-id="f86e1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f86e1-144">DateTimeOffset</span></span>|<span data-ttu-id="f86e1-145">При последнем возвращенном Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="f86e1-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="f86e1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f86e1-146">Response</span></span>
<span data-ttu-id="f86e1-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f86e1-147">If successful, this method returns a `201 Created` response code and a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f86e1-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f86e1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="f86e1-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f86e1-149">Request</span></span>
<span data-ttu-id="f86e1-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f86e1-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f86e1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f86e1-151">Response</span></span>
<span data-ttu-id="f86e1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f86e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




