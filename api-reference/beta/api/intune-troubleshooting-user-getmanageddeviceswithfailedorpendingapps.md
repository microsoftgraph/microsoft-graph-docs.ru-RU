---
title: getManagedDevicesWithFailedOrPendingApps
description: Извлечение списка устройств с сбойными или ожидающих приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 101e7335aebcfc224751bbcbc9e848971abd1e5c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134090"
---
# <a name="getmanageddeviceswithfailedorpendingapps-function"></a><span data-ttu-id="d9e85-103">getManagedDevicesWithFailedOrPendingApps</span><span class="sxs-lookup"><span data-stu-id="d9e85-103">getManagedDevicesWithFailedOrPendingApps function</span></span>

<span data-ttu-id="d9e85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e85-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e85-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9e85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e85-107">Извлечение списка устройств с сбойными или ожидающих приложениями</span><span class="sxs-lookup"><span data-stu-id="d9e85-107">Retrieves the list of devices with failed or pending apps</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9e85-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9e85-108">Prerequisites</span></span>
<span data-ttu-id="d9e85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e85-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9e85-111">Permission type</span></span>|<span data-ttu-id="d9e85-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9e85-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e85-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9e85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e85-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e85-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d9e85-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9e85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e85-116">Not supported.</span></span>|
|<span data-ttu-id="d9e85-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d9e85-117">Application</span></span>|<span data-ttu-id="d9e85-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e85-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e85-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9e85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

## <a name="request-headers"></a><span data-ttu-id="d9e85-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d9e85-120">Request headers</span></span>
|<span data-ttu-id="d9e85-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9e85-121">Header</span></span>|<span data-ttu-id="d9e85-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9e85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e85-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9e85-123">Authorization</span></span>|<span data-ttu-id="d9e85-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9e85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e85-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9e85-125">Accept</span></span>|<span data-ttu-id="d9e85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e85-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9e85-127">Request body</span></span>
<span data-ttu-id="d9e85-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9e85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9e85-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e85-129">Response</span></span>
<span data-ttu-id="d9e85-130">В случае успешной работы эта функция возвращает код ответа и `200 OK` [коллекцию managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d9e85-130">If successful, this function returns a `200 OK` response code and a [managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e85-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d9e85-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9e85-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9e85-132">Request</span></span>
<span data-ttu-id="d9e85-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9e85-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

### <a name="response"></a><span data-ttu-id="d9e85-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e85-134">Response</span></span>
<span data-ttu-id="d9e85-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9e85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 187

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState",
      "summarizedAppState": "success",
      "deviceId": "Device Id value"
    }
  ]
}
```




