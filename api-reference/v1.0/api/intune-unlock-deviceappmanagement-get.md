---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3378ea29a16408fd255160f8d596593601229b94
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755467"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="52b9d-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="52b9d-103">Get deviceAppManagement</span></span>

<span data-ttu-id="52b9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52b9d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52b9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52b9d-106">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="52b9d-106">Read properties and relationships of the [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52b9d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="52b9d-107">Prerequisites</span></span>
<span data-ttu-id="52b9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52b9d-110">Permission type</span></span>|<span data-ttu-id="52b9d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52b9d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52b9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52b9d-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b9d-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52b9d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52b9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52b9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b9d-115">Not supported.</span></span>|
|<span data-ttu-id="52b9d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="52b9d-116">Application</span></span>|<span data-ttu-id="52b9d-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b9d-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52b9d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52b9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52b9d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52b9d-119">Optional query parameters</span></span>
<span data-ttu-id="52b9d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52b9d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52b9d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52b9d-121">Request headers</span></span>
|<span data-ttu-id="52b9d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52b9d-122">Header</span></span>|<span data-ttu-id="52b9d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="52b9d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52b9d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="52b9d-124">Authorization</span></span>|<span data-ttu-id="52b9d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52b9d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52b9d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="52b9d-126">Accept</span></span>|<span data-ttu-id="52b9d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="52b9d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b9d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52b9d-128">Request body</span></span>
<span data-ttu-id="52b9d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52b9d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52b9d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b9d-130">Response</span></span>
<span data-ttu-id="52b9d-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="52b9d-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52b9d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="52b9d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="52b9d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="52b9d-133">Request</span></span>
<span data-ttu-id="52b9d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52b9d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="52b9d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b9d-135">Response</span></span>
<span data-ttu-id="52b9d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52b9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```




