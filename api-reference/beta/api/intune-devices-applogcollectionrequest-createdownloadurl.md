---
title: Действие createDownloadUrl
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d3c3a46b47d45d80532697aa7c900b74c40c57e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150656"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="75eb2-103">Действие createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="75eb2-103">createDownloadUrl action</span></span>

<span data-ttu-id="75eb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75eb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75eb2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75eb2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75eb2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75eb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75eb2-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="75eb2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75eb2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75eb2-108">Prerequisites</span></span>
<span data-ttu-id="75eb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75eb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75eb2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75eb2-111">Permission type</span></span>|<span data-ttu-id="75eb2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75eb2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75eb2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75eb2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75eb2-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75eb2-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="75eb2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75eb2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75eb2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75eb2-116">Not supported.</span></span>|
|<span data-ttu-id="75eb2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="75eb2-117">Application</span></span>|<span data-ttu-id="75eb2-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75eb2-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75eb2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75eb2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="75eb2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75eb2-120">Request headers</span></span>
|<span data-ttu-id="75eb2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75eb2-121">Header</span></span>|<span data-ttu-id="75eb2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75eb2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75eb2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75eb2-123">Authorization</span></span>|<span data-ttu-id="75eb2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75eb2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75eb2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75eb2-125">Accept</span></span>|<span data-ttu-id="75eb2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75eb2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75eb2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75eb2-127">Request body</span></span>
<span data-ttu-id="75eb2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75eb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75eb2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="75eb2-129">Response</span></span>
<span data-ttu-id="75eb2-130">В случае успешного завершения это действие возвращает код отклика и `200 OK` [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75eb2-130">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75eb2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="75eb2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="75eb2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="75eb2-132">Request</span></span>
<span data-ttu-id="75eb2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75eb2-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="75eb2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="75eb2-134">Response</span></span>
<span data-ttu-id="75eb2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75eb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails",
    "downloadUrl": "https://example.com/downloadUrl/",
    "decryptionKey": "Decryption Key value",
    "appLogDecryptionAlgorithm": "aes256"
  }
}
```




