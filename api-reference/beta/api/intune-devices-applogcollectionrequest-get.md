---
title: Получение appLogCollectionRequest
description: Чтение свойств и связей объекта appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea1443a28e85637e1908afa8ea88ab6a1844f860
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731248"
---
# <a name="get-applogcollectionrequest"></a><span data-ttu-id="10fce-103">Получение appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="10fce-103">Get appLogCollectionRequest</span></span>

<span data-ttu-id="10fce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10fce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10fce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10fce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10fce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10fce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10fce-107">Чтение свойств и связей объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="10fce-107">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10fce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10fce-108">Prerequisites</span></span>
<span data-ttu-id="10fce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10fce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10fce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10fce-111">Permission type</span></span>|<span data-ttu-id="10fce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10fce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10fce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10fce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10fce-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="10fce-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="10fce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10fce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10fce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10fce-116">Not supported.</span></span>|
|<span data-ttu-id="10fce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10fce-117">Application</span></span>|<span data-ttu-id="10fce-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="10fce-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10fce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10fce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10fce-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10fce-120">Optional query parameters</span></span>
<span data-ttu-id="10fce-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10fce-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10fce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10fce-122">Request headers</span></span>
|<span data-ttu-id="10fce-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10fce-123">Header</span></span>|<span data-ttu-id="10fce-124">Значение</span><span class="sxs-lookup"><span data-stu-id="10fce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10fce-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10fce-125">Authorization</span></span>|<span data-ttu-id="10fce-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10fce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10fce-127">Accept</span><span class="sxs-lookup"><span data-stu-id="10fce-127">Accept</span></span>|<span data-ttu-id="10fce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10fce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10fce-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10fce-129">Request body</span></span>
<span data-ttu-id="10fce-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10fce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10fce-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="10fce-131">Response</span></span>
<span data-ttu-id="10fce-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10fce-132">If successful, this method returns a `200 OK` response code and [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10fce-133">Пример</span><span class="sxs-lookup"><span data-stu-id="10fce-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="10fce-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="10fce-134">Request</span></span>
<span data-ttu-id="10fce-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10fce-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

### <a name="response"></a><span data-ttu-id="10fce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="10fce-136">Response</span></span>
<span data-ttu-id="10fce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10fce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.appLogCollectionRequest",
    "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
    "status": "completed",
    "errorMessage": "Error Message value",
    "customLogFolders": [
      "Custom Log Folders value"
    ],
    "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
  }
}
```





