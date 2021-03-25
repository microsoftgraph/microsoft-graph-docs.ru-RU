---
title: List deviceManagementDomainJoinConnectors
description: Список свойств и связей объектов deviceManagementDomainJoinConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49f4ed483655eebb9cb93a3e7e0418e241423d7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152749"
---
# <a name="list-devicemanagementdomainjoinconnectors"></a><span data-ttu-id="e8e1e-103">List deviceManagementDomainJoinConnectors</span><span class="sxs-lookup"><span data-stu-id="e8e1e-103">List deviceManagementDomainJoinConnectors</span></span>

<span data-ttu-id="e8e1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8e1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8e1e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8e1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8e1e-107">Список свойств и связей объектов [deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)</span><span class="sxs-lookup"><span data-stu-id="e8e1e-107">List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8e1e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8e1e-108">Prerequisites</span></span>
<span data-ttu-id="e8e1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8e1e-111">Permission type</span></span>|<span data-ttu-id="e8e1e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8e1e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8e1e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8e1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8e1e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e1e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8e1e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8e1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8e1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-116">Not supported.</span></span>|
|<span data-ttu-id="e8e1e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8e1e-117">Application</span></span>|<span data-ttu-id="e8e1e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e1e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8e1e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8e1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="e8e1e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8e1e-120">Request headers</span></span>
|<span data-ttu-id="e8e1e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8e1e-121">Header</span></span>|<span data-ttu-id="e8e1e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8e1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8e1e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8e1e-123">Authorization</span></span>|<span data-ttu-id="e8e1e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8e1e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8e1e-125">Accept</span></span>|<span data-ttu-id="e8e1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8e1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e1e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8e1e-127">Request body</span></span>
<span data-ttu-id="e8e1e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8e1e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e1e-129">Response</span></span>
<span data-ttu-id="e8e1e-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e1e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e8e1e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8e1e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8e1e-132">Request</span></span>
<span data-ttu-id="e8e1e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
```

### <a name="response"></a><span data-ttu-id="e8e1e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e1e-134">Response</span></span>
<span data-ttu-id="e8e1e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8e1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
      "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
      "displayName": "Display Name value",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "error",
      "version": "Version value"
    }
  ]
}
```




