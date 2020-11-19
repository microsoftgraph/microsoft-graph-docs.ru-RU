---
title: Действие createDownloadUrl
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e9ab5b0e1d780a64f533026d492ffa9ce0e0e02
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286180"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="4404f-103">Действие createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="4404f-103">createDownloadUrl action</span></span>

<span data-ttu-id="4404f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4404f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4404f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4404f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4404f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4404f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4404f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4404f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4404f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4404f-108">Prerequisites</span></span>
<span data-ttu-id="4404f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4404f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4404f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4404f-111">Permission type</span></span>|<span data-ttu-id="4404f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4404f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4404f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4404f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4404f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4404f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4404f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4404f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4404f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4404f-116">Not supported.</span></span>|
|<span data-ttu-id="4404f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4404f-117">Application</span></span>|<span data-ttu-id="4404f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4404f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4404f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4404f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="4404f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4404f-120">Request headers</span></span>
|<span data-ttu-id="4404f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4404f-121">Header</span></span>|<span data-ttu-id="4404f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4404f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4404f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4404f-123">Authorization</span></span>|<span data-ttu-id="4404f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4404f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4404f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4404f-125">Accept</span></span>|<span data-ttu-id="4404f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4404f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4404f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4404f-127">Request body</span></span>
<span data-ttu-id="4404f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4404f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4404f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4404f-129">Response</span></span>
<span data-ttu-id="4404f-130">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [апплогколлектиондовнлоаддетаилс](../resources/intune-devices-applogcollectiondownloaddetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4404f-130">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4404f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4404f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4404f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4404f-132">Request</span></span>
<span data-ttu-id="4404f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4404f-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="4404f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4404f-134">Response</span></span>
<span data-ttu-id="4404f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4404f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




