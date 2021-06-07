---
title: Get managedAppStatusRaw
description: Чтение свойств и связей объекта managedAppStatusRaw.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34c67b11e68954cbc3d2ce38798e2a4b22d7f28b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756122"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="e2552-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="e2552-103">Get managedAppStatusRaw</span></span>

<span data-ttu-id="e2552-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2552-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2552-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2552-106">Чтение свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="e2552-106">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2552-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e2552-107">Prerequisites</span></span>
<span data-ttu-id="e2552-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2552-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2552-110">Permission type</span></span>|<span data-ttu-id="e2552-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2552-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2552-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2552-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2552-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2552-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2552-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2552-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2552-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2552-115">Not supported.</span></span>|
|<span data-ttu-id="e2552-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e2552-116">Application</span></span>|<span data-ttu-id="e2552-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2552-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2552-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2552-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2552-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2552-119">Optional query parameters</span></span>
<span data-ttu-id="e2552-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2552-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2552-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2552-121">Request headers</span></span>
|<span data-ttu-id="e2552-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2552-122">Header</span></span>|<span data-ttu-id="e2552-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e2552-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2552-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2552-124">Authorization</span></span>|<span data-ttu-id="e2552-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2552-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2552-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e2552-126">Accept</span></span>|<span data-ttu-id="e2552-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2552-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2552-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2552-128">Request body</span></span>
<span data-ttu-id="e2552-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2552-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2552-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2552-130">Response</span></span>
<span data-ttu-id="e2552-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e2552-131">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2552-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e2552-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2552-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2552-133">Request</span></span>
<span data-ttu-id="e2552-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2552-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="e2552-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2552-135">Response</span></span>
<span data-ttu-id="e2552-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```




