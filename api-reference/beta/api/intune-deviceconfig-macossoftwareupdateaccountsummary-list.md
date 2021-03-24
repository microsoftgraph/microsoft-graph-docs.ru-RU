---
title: Список macOSSoftwareUpdateAccountSummaries
description: Список свойств и связей объектов macOSSoftwareUpdateAccountSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a6da845494a1401625ffcbf42fd471dd019d3ec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129736"
---
# <a name="list-macossoftwareupdateaccountsummaries"></a><span data-ttu-id="424eb-103">Список macOSSoftwareUpdateAccountSummaries</span><span class="sxs-lookup"><span data-stu-id="424eb-103">List macOSSoftwareUpdateAccountSummaries</span></span>

<span data-ttu-id="424eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="424eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="424eb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="424eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="424eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="424eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="424eb-107">Список свойств и связей объектов [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)</span><span class="sxs-lookup"><span data-stu-id="424eb-107">List properties and relationships of the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="424eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="424eb-108">Prerequisites</span></span>
<span data-ttu-id="424eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="424eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="424eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="424eb-111">Permission type</span></span>|<span data-ttu-id="424eb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="424eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="424eb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="424eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="424eb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="424eb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="424eb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="424eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="424eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="424eb-116">Not supported.</span></span>|
|<span data-ttu-id="424eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="424eb-117">Application</span></span>|<span data-ttu-id="424eb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="424eb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="424eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="424eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/macOSSoftwareUpdateAccountSummaries
```

## <a name="request-headers"></a><span data-ttu-id="424eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="424eb-120">Request headers</span></span>
|<span data-ttu-id="424eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="424eb-121">Header</span></span>|<span data-ttu-id="424eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="424eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="424eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="424eb-123">Authorization</span></span>|<span data-ttu-id="424eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="424eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="424eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="424eb-125">Accept</span></span>|<span data-ttu-id="424eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="424eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="424eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="424eb-127">Request body</span></span>
<span data-ttu-id="424eb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="424eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="424eb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="424eb-129">Response</span></span>
<span data-ttu-id="424eb-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="424eb-130">If successful, this method returns a `200 OK` response code and a collection of [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="424eb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="424eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="424eb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="424eb-132">Request</span></span>
<span data-ttu-id="424eb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="424eb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries
```

### <a name="response"></a><span data-ttu-id="424eb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="424eb-134">Response</span></span>
<span data-ttu-id="424eb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="424eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 583

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
      "id": "64687d05-7d05-6468-057d-6864057d6864",
      "displayName": "Display Name value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceName": "Device Name value",
      "userPrincipalName": "User Principal Name value",
      "osVersion": "Os Version value",
      "successfulUpdateCount": 5,
      "failedUpdateCount": 1,
      "totalUpdateCount": 0,
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




