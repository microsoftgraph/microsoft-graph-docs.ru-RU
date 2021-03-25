---
title: функция getComanagedDevicesSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f46d9f9baecf9639966ba08c745fa23ee84cb923
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154345"
---
# <a name="getcomanageddevicessummary-function"></a><span data-ttu-id="53426-103">функция getComanagedDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="53426-103">getComanagedDevicesSummary function</span></span>

<span data-ttu-id="53426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53426-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53426-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53426-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53426-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53426-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53426-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="53426-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53426-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53426-108">Prerequisites</span></span>
<span data-ttu-id="53426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53426-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53426-111">Permission type</span></span>|<span data-ttu-id="53426-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53426-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53426-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53426-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53426-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53426-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53426-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53426-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53426-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53426-116">Not supported.</span></span>|
|<span data-ttu-id="53426-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="53426-117">Application</span></span>|<span data-ttu-id="53426-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53426-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53426-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53426-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagedDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="53426-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53426-120">Request headers</span></span>
|<span data-ttu-id="53426-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53426-121">Header</span></span>|<span data-ttu-id="53426-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53426-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53426-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53426-123">Authorization</span></span>|<span data-ttu-id="53426-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53426-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53426-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53426-125">Accept</span></span>|<span data-ttu-id="53426-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53426-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53426-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53426-127">Request body</span></span>
<span data-ttu-id="53426-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53426-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53426-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="53426-129">Response</span></span>
<span data-ttu-id="53426-130">В случае успешной работы эта функция возвращает код ответа и `200 OK` [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="53426-130">If successful, this function returns a `200 OK` response code and a [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53426-131">Пример</span><span class="sxs-lookup"><span data-stu-id="53426-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="53426-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="53426-132">Request</span></span>
<span data-ttu-id="53426-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53426-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagedDevicesSummary
```

### <a name="response"></a><span data-ttu-id="53426-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="53426-134">Response</span></span>
<span data-ttu-id="53426-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53426-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": {
    "@odata.type": "microsoft.graph.comanagedDevicesSummary",
    "inventoryCount": 14,
    "compliancePolicyCount": 5,
    "resourceAccessCount": 3,
    "configurationSettingsCount": 10,
    "windowsUpdateForBusinessCount": 13,
    "endpointProtectionCount": 7,
    "modernAppsCount": 15,
    "officeAppsCount": 15,
    "totalComanagedCount": 3
  }
}
```




