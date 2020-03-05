---
title: Список Девицеманажементдомаинжоинконнекторс
description: Список свойств и связей объектов Девицеманажементдомаинжоинконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e0708c0931f8f1028afd7f96ff34b0d87dcec72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462553"
---
# <a name="list-devicemanagementdomainjoinconnectors"></a><span data-ttu-id="e95e8-103">Список Девицеманажементдомаинжоинконнекторс</span><span class="sxs-lookup"><span data-stu-id="e95e8-103">List deviceManagementDomainJoinConnectors</span></span>

<span data-ttu-id="e95e8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e95e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e95e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e95e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e95e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e95e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e95e8-107">Список свойств и связей объектов [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="e95e8-107">List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e95e8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e95e8-108">Prerequisites</span></span>
<span data-ttu-id="e95e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e95e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e95e8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e95e8-111">Permission type</span></span>|<span data-ttu-id="e95e8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e95e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e95e8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e95e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e95e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e95e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e95e8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e95e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e95e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e95e8-116">Not supported.</span></span>|
|<span data-ttu-id="e95e8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e95e8-117">Application</span></span>|<span data-ttu-id="e95e8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e95e8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e95e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e95e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="e95e8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e95e8-120">Request headers</span></span>
|<span data-ttu-id="e95e8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e95e8-121">Header</span></span>|<span data-ttu-id="e95e8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e95e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e95e8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e95e8-123">Authorization</span></span>|<span data-ttu-id="e95e8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e95e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e95e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e95e8-125">Accept</span></span>|<span data-ttu-id="e95e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e95e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e95e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e95e8-127">Request body</span></span>
<span data-ttu-id="e95e8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e95e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e95e8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e95e8-129">Response</span></span>
<span data-ttu-id="e95e8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e95e8-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e95e8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e95e8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e95e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e95e8-132">Request</span></span>
<span data-ttu-id="e95e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e95e8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
```

### <a name="response"></a><span data-ttu-id="e95e8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e95e8-134">Response</span></span>
<span data-ttu-id="e95e8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e95e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





