---
title: Get cloudPCConnectivityIssue
description: Чтение свойств и связей объекта cloudPCConnectivityIssue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0a6595d833cb973deb460f39724010a7f70501f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664877"
---
# <a name="get-cloudpcconnectivityissue"></a><span data-ttu-id="77127-103">Get cloudPCConnectivityIssue</span><span class="sxs-lookup"><span data-stu-id="77127-103">Get cloudPCConnectivityIssue</span></span>

<span data-ttu-id="77127-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77127-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77127-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77127-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77127-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77127-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77127-107">Чтение свойств и связей объекта [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="77127-107">Read properties and relationships of the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77127-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77127-108">Prerequisites</span></span>
<span data-ttu-id="77127-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77127-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77127-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77127-111">Permission type</span></span>|<span data-ttu-id="77127-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77127-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77127-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77127-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77127-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77127-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77127-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77127-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77127-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77127-116">Not supported.</span></span>|
|<span data-ttu-id="77127-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77127-117">Application</span></span>|<span data-ttu-id="77127-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77127-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77127-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77127-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77127-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77127-120">Optional query parameters</span></span>
<span data-ttu-id="77127-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77127-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77127-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77127-122">Request headers</span></span>
|<span data-ttu-id="77127-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77127-123">Header</span></span>|<span data-ttu-id="77127-124">Значение</span><span class="sxs-lookup"><span data-stu-id="77127-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77127-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="77127-125">Authorization</span></span>|<span data-ttu-id="77127-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77127-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77127-127">Accept</span><span class="sxs-lookup"><span data-stu-id="77127-127">Accept</span></span>|<span data-ttu-id="77127-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77127-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77127-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77127-129">Request body</span></span>
<span data-ttu-id="77127-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77127-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77127-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="77127-131">Response</span></span>
<span data-ttu-id="77127-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="77127-132">If successful, this method returns a `200 OK` response code and [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77127-133">Пример</span><span class="sxs-lookup"><span data-stu-id="77127-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="77127-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="77127-134">Request</span></span>
<span data-ttu-id="77127-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77127-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

### <a name="response"></a><span data-ttu-id="77127-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="77127-136">Response</span></span>
<span data-ttu-id="77127-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77127-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
    "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
    "deviceId": "Device Id value",
    "errorCode": "Error Code value",
    "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
    "userId": "User Id value",
    "errorDescription": "Error Description value",
    "recommendedAction": "Recommended Action value"
  }
}
```




