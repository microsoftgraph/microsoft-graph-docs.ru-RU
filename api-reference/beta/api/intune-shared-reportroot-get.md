---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19dda54fa81f60607a8ea816c65a3a6367a78233
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261932"
---
# <a name="get-reportroot"></a><span data-ttu-id="68c62-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="68c62-103">Get reportRoot</span></span>

<span data-ttu-id="68c62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68c62-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="68c62-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68c62-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c62-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68c62-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68c62-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c62-108">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="68c62-108">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68c62-109">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="68c62-109">Prerequisites</span></span>
<span data-ttu-id="68c62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c62-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68c62-112">Permission type</span></span>|<span data-ttu-id="68c62-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68c62-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68c62-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68c62-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="68c62-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="68c62-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="68c62-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="68c62-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="68c62-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="68c62-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="68c62-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="68c62-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="68c62-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68c62-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68c62-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c62-120">Not supported.</span></span>|
|<span data-ttu-id="68c62-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="68c62-121">Application</span></span>||
| <span data-ttu-id="68c62-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="68c62-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="68c62-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="68c62-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="68c62-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="68c62-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="68c62-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="68c62-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68c62-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68c62-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68c62-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68c62-127">Optional query parameters</span></span>
<span data-ttu-id="68c62-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="68c62-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68c62-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68c62-129">Request headers</span></span>
|<span data-ttu-id="68c62-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68c62-130">Header</span></span>|<span data-ttu-id="68c62-131">Значение</span><span class="sxs-lookup"><span data-stu-id="68c62-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68c62-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68c62-132">Authorization</span></span>|<span data-ttu-id="68c62-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68c62-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68c62-134">Accept</span><span class="sxs-lookup"><span data-stu-id="68c62-134">Accept</span></span>|<span data-ttu-id="68c62-135">application/json</span><span class="sxs-lookup"><span data-stu-id="68c62-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68c62-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68c62-136">Request body</span></span>
<span data-ttu-id="68c62-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68c62-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68c62-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c62-138">Response</span></span>
<span data-ttu-id="68c62-139">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="68c62-139">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68c62-140">Пример</span><span class="sxs-lookup"><span data-stu-id="68c62-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="68c62-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c62-141">Request</span></span>
<span data-ttu-id="68c62-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c62-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="68c62-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c62-143">Response</span></span>
<span data-ttu-id="68c62-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c62-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










