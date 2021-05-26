---
title: Список cloudPCConnectivityIssues
description: Список свойств и связей объектов cloudPCConnectivityIssue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18260210f30c6b0728d4d2f3d85e55910bb802f9
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664840"
---
# <a name="list-cloudpcconnectivityissues"></a><span data-ttu-id="f3fca-103">Список cloudPCConnectivityIssues</span><span class="sxs-lookup"><span data-stu-id="f3fca-103">List cloudPCConnectivityIssues</span></span>

<span data-ttu-id="f3fca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3fca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3fca-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3fca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3fca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3fca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3fca-107">Список свойств и связей объектов [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="f3fca-107">List properties and relationships of the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3fca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3fca-108">Prerequisites</span></span>
<span data-ttu-id="f3fca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3fca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3fca-111">Permission type</span></span>|<span data-ttu-id="f3fca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3fca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3fca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3fca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3fca-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fca-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3fca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3fca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3fca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3fca-116">Not supported.</span></span>|
|<span data-ttu-id="f3fca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3fca-117">Application</span></span>|<span data-ttu-id="f3fca-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fca-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3fca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3fca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cloudPCConnectivityIssues
```

## <a name="request-headers"></a><span data-ttu-id="f3fca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3fca-120">Request headers</span></span>
|<span data-ttu-id="f3fca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3fca-121">Header</span></span>|<span data-ttu-id="f3fca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3fca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3fca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3fca-123">Authorization</span></span>|<span data-ttu-id="f3fca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3fca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3fca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3fca-125">Accept</span></span>|<span data-ttu-id="f3fca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3fca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3fca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3fca-127">Request body</span></span>
<span data-ttu-id="f3fca-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3fca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3fca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3fca-129">Response</span></span>
<span data-ttu-id="f3fca-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3fca-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3fca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f3fca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3fca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3fca-132">Request</span></span>
<span data-ttu-id="f3fca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3fca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues
```

### <a name="response"></a><span data-ttu-id="f3fca-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3fca-134">Response</span></span>
<span data-ttu-id="f3fca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3fca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
      "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
      "deviceId": "Device Id value",
      "errorCode": "Error Code value",
      "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
      "userId": "User Id value",
      "errorDescription": "Error Description value",
      "recommendedAction": "Recommended Action value"
    }
  ]
}
```




