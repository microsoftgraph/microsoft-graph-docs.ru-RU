---
title: Создание microsoftTunnelServer
description: Создание нового объекта microsoftTunnelServer.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9636422495a2c7834dc7ed678c49a389e16b0df9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141801"
---
# <a name="create-microsofttunnelserver"></a><span data-ttu-id="bdcb2-103">Создание microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="bdcb2-103">Create microsoftTunnelServer</span></span>

<span data-ttu-id="bdcb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdcb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdcb2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdcb2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdcb2-107">Создание нового [объекта microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)</span><span class="sxs-lookup"><span data-stu-id="bdcb2-107">Create a new [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdcb2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bdcb2-108">Prerequisites</span></span>
<span data-ttu-id="bdcb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdcb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdcb2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdcb2-111">Permission type</span></span>|<span data-ttu-id="bdcb2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdcb2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdcb2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdcb2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdcb2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcb2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdcb2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdcb2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdcb2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-116">Not supported.</span></span>|
|<span data-ttu-id="bdcb2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bdcb2-117">Application</span></span>|<span data-ttu-id="bdcb2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcb2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdcb2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdcb2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a><span data-ttu-id="bdcb2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bdcb2-120">Request headers</span></span>
|<span data-ttu-id="bdcb2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdcb2-121">Header</span></span>|<span data-ttu-id="bdcb2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdcb2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdcb2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdcb2-123">Authorization</span></span>|<span data-ttu-id="bdcb2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdcb2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdcb2-125">Accept</span></span>|<span data-ttu-id="bdcb2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdcb2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdcb2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdcb2-127">Request body</span></span>
<span data-ttu-id="bdcb2-128">В теле запроса поставляем представление JSON для объекта microsoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-128">In the request body, supply a JSON representation for the microsoftTunnelServer object.</span></span>

<span data-ttu-id="bdcb2-129">В следующей таблице показаны свойства, необходимые при создании microsoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-129">The following table shows the properties that are required when you create the microsoftTunnelServer.</span></span>

|<span data-ttu-id="bdcb2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdcb2-130">Property</span></span>|<span data-ttu-id="bdcb2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bdcb2-131">Type</span></span>|<span data-ttu-id="bdcb2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bdcb2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdcb2-133">id</span><span class="sxs-lookup"><span data-stu-id="bdcb2-133">id</span></span>|<span data-ttu-id="bdcb2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bdcb2-134">String</span></span>|<span data-ttu-id="bdcb2-135">Id MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="bdcb2-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="bdcb2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bdcb2-136">displayName</span></span>|<span data-ttu-id="bdcb2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="bdcb2-137">String</span></span>|<span data-ttu-id="bdcb2-138">Имя отображения MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="bdcb2-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="bdcb2-139">tunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="bdcb2-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="bdcb2-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="bdcb2-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="bdcb2-141">Состояние здоровья MicrosoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="bdcb2-142">Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="bdcb2-143">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="bdcb2-143">lastCheckinDateTime</span></span>|<span data-ttu-id="bdcb2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdcb2-144">DateTimeOffset</span></span>|<span data-ttu-id="bdcb2-145">При последней регистрации в MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="bdcb2-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="bdcb2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdcb2-146">Response</span></span>
<span data-ttu-id="bdcb2-147">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект MicrosoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-147">If successful, this method returns a `201 Created` response code and a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdcb2-148">Пример</span><span class="sxs-lookup"><span data-stu-id="bdcb2-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdcb2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdcb2-149">Request</span></span>
<span data-ttu-id="bdcb2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bdcb2-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdcb2-151">Response</span></span>
<span data-ttu-id="bdcb2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdcb2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




