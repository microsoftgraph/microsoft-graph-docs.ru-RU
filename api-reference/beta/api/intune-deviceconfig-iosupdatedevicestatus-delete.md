---
title: Удаление объекта iosUpdateDeviceStatus
description: Удаляет объект iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 960aa60b28d723b4b6051d6bb66110869af00024
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131402"
---
# <a name="delete-iosupdatedevicestatus"></a><span data-ttu-id="71058-103">Удаление объекта iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="71058-103">Delete iosUpdateDeviceStatus</span></span>

<span data-ttu-id="71058-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71058-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71058-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71058-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71058-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71058-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71058-107">Удаляет объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="71058-107">Deletes a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71058-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71058-108">Prerequisites</span></span>
<span data-ttu-id="71058-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71058-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71058-111">Permission type</span></span>|<span data-ttu-id="71058-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71058-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71058-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71058-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71058-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71058-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71058-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71058-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71058-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71058-116">Not supported.</span></span>|
|<span data-ttu-id="71058-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="71058-117">Application</span></span>|<span data-ttu-id="71058-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71058-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71058-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71058-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="71058-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71058-120">Request headers</span></span>
|<span data-ttu-id="71058-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71058-121">Header</span></span>|<span data-ttu-id="71058-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71058-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71058-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71058-123">Authorization</span></span>|<span data-ttu-id="71058-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71058-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71058-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71058-125">Accept</span></span>|<span data-ttu-id="71058-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71058-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71058-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71058-127">Request body</span></span>
<span data-ttu-id="71058-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71058-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71058-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71058-129">Response</span></span>
<span data-ttu-id="71058-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71058-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71058-131">Пример</span><span class="sxs-lookup"><span data-stu-id="71058-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="71058-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71058-132">Request</span></span>
<span data-ttu-id="71058-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71058-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="71058-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="71058-134">Response</span></span>
<span data-ttu-id="71058-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




