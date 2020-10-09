---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bba1f299aec5a896796c045067c3d6f8c5eaa425
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405052"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="bd5b5-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="bd5b5-103">Get deviceAppManagement</span></span>

<span data-ttu-id="bd5b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd5b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd5b5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd5b5-106">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="bd5b5-106">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd5b5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5b5-107">Prerequisites</span></span>

<span data-ttu-id="bd5b5-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bd5b5-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5b5-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="bd5b5-110">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="bd5b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5b5-111">Permission type</span></span>|<span data-ttu-id="bd5b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd5b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd5b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd5b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd5b5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd5b5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="bd5b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd5b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd5b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-116">Not supported.</span></span>|
|<span data-ttu-id="bd5b5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd5b5-117">Application</span></span>|<span data-ttu-id="bd5b5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd5b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd5b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd5b5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd5b5-120">Optional query parameters</span></span>
<span data-ttu-id="bd5b5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd5b5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd5b5-122">Request headers</span></span>
|<span data-ttu-id="bd5b5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd5b5-123">Header</span></span>|<span data-ttu-id="bd5b5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bd5b5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd5b5-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd5b5-125">Authorization</span></span>|<span data-ttu-id="bd5b5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd5b5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bd5b5-127">Accept</span></span>|<span data-ttu-id="bd5b5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bd5b5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5b5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd5b5-129">Request body</span></span>
<span data-ttu-id="bd5b5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd5b5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5b5-131">Response</span></span>
<span data-ttu-id="bd5b5-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-132">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="bd5b5-133">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="bd5b5-133">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="bd5b5-134">Пример отклика</span><span class="sxs-lookup"><span data-stu-id="bd5b5-134">Example response</span></span>
<span data-ttu-id="bd5b5-135">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-135">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bd5b5-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd5b5-136">All properties will be returned from an actual call.</span></span>

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