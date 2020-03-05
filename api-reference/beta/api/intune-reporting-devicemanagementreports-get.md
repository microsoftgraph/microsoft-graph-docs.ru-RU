---
title: Получение Девицеманажементрепортс
description: Чтение свойств и связей объекта Девицеманажементрепортс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e439ce9c2a864b9901590dab70ffab309d9e50d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459178"
---
# <a name="get-devicemanagementreports"></a><span data-ttu-id="9e679-103">Получение Девицеманажементрепортс</span><span class="sxs-lookup"><span data-stu-id="9e679-103">Get deviceManagementReports</span></span>

<span data-ttu-id="9e679-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9e679-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e679-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e679-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e679-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e679-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e679-107">Чтение свойств и связей объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="9e679-107">Read properties and relationships of the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e679-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9e679-108">Prerequisites</span></span>
<span data-ttu-id="9e679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e679-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e679-111">Permission type</span></span>|<span data-ttu-id="9e679-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e679-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e679-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e679-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e679-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="9e679-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9e679-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e679-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e679-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e679-116">Not supported.</span></span>|
|<span data-ttu-id="9e679-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e679-117">Application</span></span>|<span data-ttu-id="9e679-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="9e679-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e679-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e679-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e679-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e679-120">Optional query parameters</span></span>
<span data-ttu-id="9e679-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e679-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e679-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e679-122">Request headers</span></span>
|<span data-ttu-id="9e679-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e679-123">Header</span></span>|<span data-ttu-id="9e679-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9e679-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e679-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e679-125">Authorization</span></span>|<span data-ttu-id="9e679-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e679-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e679-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9e679-127">Accept</span></span>|<span data-ttu-id="9e679-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9e679-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e679-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e679-129">Request body</span></span>
<span data-ttu-id="9e679-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e679-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e679-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e679-131">Response</span></span>
<span data-ttu-id="9e679-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e679-132">If successful, this method returns a `200 OK` response code and [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e679-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9e679-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e679-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e679-134">Request</span></span>
<span data-ttu-id="9e679-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e679-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports
```

### <a name="response"></a><span data-ttu-id="9e679-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e679-136">Response</span></span>
<span data-ttu-id="9e679-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e679-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 137

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementReports",
    "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
  }
}
```





