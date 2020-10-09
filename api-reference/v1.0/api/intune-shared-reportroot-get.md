---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d22989835a5311a1ee7f09618becc38a389975b
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406032"
---
# <a name="get-reportroot"></a><span data-ttu-id="4cad6-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="4cad6-103">Get reportRoot</span></span>

<span data-ttu-id="4cad6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cad6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cad6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cad6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cad6-106">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="4cad6-106">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cad6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4cad6-107">Prerequisites</span></span>
<span data-ttu-id="4cad6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cad6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cad6-110">Permission type</span></span>|<span data-ttu-id="4cad6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cad6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cad6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cad6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4cad6-113">&nbsp;&nbsp;Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="4cad6-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="4cad6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cad6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4cad6-115">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="4cad6-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="4cad6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cad6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4cad6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cad6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cad6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cad6-118">Not supported.</span></span>|
|<span data-ttu-id="4cad6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cad6-119">Application</span></span>|<span data-ttu-id="4cad6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cad6-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cad6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cad6-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cad6-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cad6-122">Optional query parameters</span></span>
<span data-ttu-id="4cad6-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4cad6-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4cad6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cad6-124">Request headers</span></span>
|<span data-ttu-id="4cad6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cad6-125">Header</span></span>|<span data-ttu-id="4cad6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="4cad6-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cad6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cad6-127">Authorization</span></span>|<span data-ttu-id="4cad6-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cad6-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cad6-129">Accept</span><span class="sxs-lookup"><span data-stu-id="4cad6-129">Accept</span></span>|<span data-ttu-id="4cad6-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4cad6-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cad6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cad6-131">Request body</span></span>
<span data-ttu-id="4cad6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cad6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cad6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cad6-133">Response</span></span>
<span data-ttu-id="4cad6-134">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4cad6-134">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cad6-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4cad6-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="4cad6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cad6-136">Request</span></span>
<span data-ttu-id="4cad6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cad6-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="4cad6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cad6-138">Response</span></span>
<span data-ttu-id="4cad6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cad6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```