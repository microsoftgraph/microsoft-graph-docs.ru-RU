---
title: Получение объекта softwareUpdateStatusSummary
description: Чтение свойств и связей объекта softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ae032ecb6e07c102cc7ebec7865cf56ab590731
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137093"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="e88ef-103">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e88ef-103">Get softwareUpdateStatusSummary</span></span>

<span data-ttu-id="e88ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e88ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e88ef-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e88ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e88ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e88ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e88ef-107">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="e88ef-107">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e88ef-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e88ef-108">Prerequisites</span></span>
<span data-ttu-id="e88ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e88ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e88ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e88ef-111">Permission type</span></span>|<span data-ttu-id="e88ef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e88ef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e88ef-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e88ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e88ef-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e88ef-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e88ef-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e88ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e88ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e88ef-116">Not supported.</span></span>|
|<span data-ttu-id="e88ef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e88ef-117">Application</span></span>|<span data-ttu-id="e88ef-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e88ef-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e88ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e88ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e88ef-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e88ef-120">Optional query parameters</span></span>
<span data-ttu-id="e88ef-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e88ef-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e88ef-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e88ef-122">Request headers</span></span>
|<span data-ttu-id="e88ef-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e88ef-123">Header</span></span>|<span data-ttu-id="e88ef-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e88ef-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e88ef-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e88ef-125">Authorization</span></span>|<span data-ttu-id="e88ef-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e88ef-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e88ef-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e88ef-127">Accept</span></span>|<span data-ttu-id="e88ef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e88ef-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e88ef-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e88ef-129">Request body</span></span>
<span data-ttu-id="e88ef-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e88ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e88ef-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e88ef-131">Response</span></span>
<span data-ttu-id="e88ef-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e88ef-132">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e88ef-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e88ef-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e88ef-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e88ef-134">Request</span></span>
<span data-ttu-id="e88ef-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e88ef-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="e88ef-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e88ef-136">Response</span></span>
<span data-ttu-id="e88ef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e88ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```




