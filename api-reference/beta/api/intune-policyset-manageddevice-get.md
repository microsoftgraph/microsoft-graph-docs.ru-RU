---
title: Получение managedDevice
description: Чтение свойств и связей объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a1b9144372fe8890c193d0406fbc0f0caab5140d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152399"
---
# <a name="get-manageddevice"></a><span data-ttu-id="6e371-103">Получение managedDevice</span><span class="sxs-lookup"><span data-stu-id="6e371-103">Get managedDevice</span></span>

<span data-ttu-id="6e371-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e371-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e371-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e371-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e371-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e371-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e371-107">Чтение свойств и связей объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6e371-107">Read properties and relationships of the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e371-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6e371-108">Prerequisites</span></span>
<span data-ttu-id="6e371-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e371-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e371-111">Permission type</span></span>|<span data-ttu-id="6e371-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e371-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e371-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e371-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e371-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e371-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e371-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e371-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e371-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e371-116">Not supported.</span></span>|
|<span data-ttu-id="6e371-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e371-117">Application</span></span>|<span data-ttu-id="6e371-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e371-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e371-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e371-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e371-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e371-120">Optional query parameters</span></span>
<span data-ttu-id="6e371-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6e371-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e371-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e371-122">Request headers</span></span>
|<span data-ttu-id="6e371-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e371-123">Header</span></span>|<span data-ttu-id="6e371-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6e371-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e371-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e371-125">Authorization</span></span>|<span data-ttu-id="6e371-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e371-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e371-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6e371-127">Accept</span></span>|<span data-ttu-id="6e371-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6e371-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e371-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e371-129">Request body</span></span>
<span data-ttu-id="6e371-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e371-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e371-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e371-131">Response</span></span>
<span data-ttu-id="6e371-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [managedDevice](../resources/intune-shared-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e371-132">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e371-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6e371-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e371-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e371-134">Request</span></span>
<span data-ttu-id="6e371-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e371-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="6e371-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e371-136">Response</span></span>
<span data-ttu-id="6e371-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e371-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 127

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDevice",
    "id": "705c034c-034c-705c-4c03-5c704c035c70"
  }
}
```




