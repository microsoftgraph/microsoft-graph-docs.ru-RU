---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d22989835a5311a1ee7f09618becc38a389975b
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732737"
---
# <a name="get-reportroot"></a><span data-ttu-id="3912f-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="3912f-103">Get reportRoot</span></span>

<span data-ttu-id="3912f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3912f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3912f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3912f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3912f-106">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="3912f-106">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3912f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3912f-107">Prerequisites</span></span>
<span data-ttu-id="3912f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3912f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3912f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3912f-110">Permission type</span></span>|<span data-ttu-id="3912f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3912f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3912f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3912f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3912f-113">&nbsp;&nbsp;Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="3912f-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="3912f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3912f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="3912f-115">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="3912f-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3912f-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3912f-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3912f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3912f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3912f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3912f-118">Not supported.</span></span>|
|<span data-ttu-id="3912f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3912f-119">Application</span></span>|<span data-ttu-id="3912f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3912f-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3912f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3912f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3912f-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3912f-122">Optional query parameters</span></span>
<span data-ttu-id="3912f-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3912f-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3912f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3912f-124">Request headers</span></span>
|<span data-ttu-id="3912f-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3912f-125">Header</span></span>|<span data-ttu-id="3912f-126">Значение</span><span class="sxs-lookup"><span data-stu-id="3912f-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3912f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3912f-127">Authorization</span></span>|<span data-ttu-id="3912f-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3912f-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3912f-129">Accept</span><span class="sxs-lookup"><span data-stu-id="3912f-129">Accept</span></span>|<span data-ttu-id="3912f-130">application/json</span><span class="sxs-lookup"><span data-stu-id="3912f-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3912f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3912f-131">Request body</span></span>
<span data-ttu-id="3912f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3912f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3912f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3912f-133">Response</span></span>
<span data-ttu-id="3912f-134">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3912f-134">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3912f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3912f-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="3912f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3912f-136">Request</span></span>
<span data-ttu-id="3912f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3912f-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="3912f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3912f-138">Response</span></span>
<span data-ttu-id="3912f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3912f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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