---
title: Get managedDeviceMobileAppConfigurationAssignment
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16aba571a01d3c5e8da37d5b09dd067645f24fe0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971127"
---
# <a name="get-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="67db3-103">Get managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="67db3-103">Get managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="67db3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67db3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67db3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67db3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67db3-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="67db3-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67db3-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="67db3-107">Prerequisites</span></span>
<span data-ttu-id="67db3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67db3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67db3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67db3-110">Permission type</span></span>|<span data-ttu-id="67db3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67db3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67db3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67db3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67db3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="67db3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="67db3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67db3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67db3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67db3-115">Not supported.</span></span>|
|<span data-ttu-id="67db3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67db3-116">Application</span></span>|<span data-ttu-id="67db3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67db3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67db3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67db3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67db3-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="67db3-119">Optional query parameters</span></span>
<span data-ttu-id="67db3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67db3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67db3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67db3-121">Request headers</span></span>
|<span data-ttu-id="67db3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67db3-122">Header</span></span>|<span data-ttu-id="67db3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="67db3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67db3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="67db3-124">Authorization</span></span>|<span data-ttu-id="67db3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67db3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67db3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="67db3-126">Accept</span></span>|<span data-ttu-id="67db3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="67db3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67db3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67db3-128">Request body</span></span>
<span data-ttu-id="67db3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67db3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67db3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="67db3-130">Response</span></span>
<span data-ttu-id="67db3-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="67db3-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67db3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="67db3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="67db3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="67db3-133">Request</span></span>
<span data-ttu-id="67db3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67db3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="67db3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="67db3-135">Response</span></span>
<span data-ttu-id="67db3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67db3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
    "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```









