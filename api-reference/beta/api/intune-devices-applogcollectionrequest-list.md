---
title: Список appLogCollectionRequests
description: Список свойств и связей объектов appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1ade110b94bea678db2fc15016aafd05e9ca51b
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612284"
---
# <a name="list-applogcollectionrequests"></a><span data-ttu-id="cb76a-103">Список appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="cb76a-103">List appLogCollectionRequests</span></span>

<span data-ttu-id="cb76a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb76a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb76a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb76a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb76a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb76a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb76a-107">Список свойств и связей объектов [appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="cb76a-107">List properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb76a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb76a-108">Prerequisites</span></span>
<span data-ttu-id="cb76a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb76a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb76a-111">Permission type</span></span>|<span data-ttu-id="cb76a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb76a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb76a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb76a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb76a-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb76a-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb76a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb76a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb76a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb76a-116">Not supported.</span></span>|
|<span data-ttu-id="cb76a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb76a-117">Application</span></span>|<span data-ttu-id="cb76a-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb76a-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb76a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb76a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="cb76a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb76a-120">Request headers</span></span>
|<span data-ttu-id="cb76a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb76a-121">Header</span></span>|<span data-ttu-id="cb76a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb76a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb76a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb76a-123">Authorization</span></span>|<span data-ttu-id="cb76a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb76a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb76a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb76a-125">Accept</span></span>|<span data-ttu-id="cb76a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb76a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb76a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb76a-127">Request body</span></span>
<span data-ttu-id="cb76a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb76a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb76a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb76a-129">Response</span></span>
<span data-ttu-id="cb76a-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb76a-130">If successful, this method returns a `200 OK` response code and a collection of [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb76a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb76a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb76a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb76a-132">Request</span></span>
<span data-ttu-id="cb76a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb76a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

### <a name="response"></a><span data-ttu-id="cb76a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb76a-134">Response</span></span>
<span data-ttu-id="cb76a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb76a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appLogCollectionRequest",
      "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
      "status": "completed",
      "errorMessage": "Error Message value",
      "customLogFolders": [
        "Custom Log Folders value"
      ],
      "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
    }
  ]
}
```




