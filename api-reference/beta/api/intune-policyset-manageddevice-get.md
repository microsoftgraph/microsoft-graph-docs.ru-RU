---
title: Получение managedDevice
description: Чтение свойств и связей объекта managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdcbb3cc8bd9aa34848768d83191ff42683a2b04
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160583"
---
# <a name="get-manageddevice"></a><span data-ttu-id="55a30-103">Получение managedDevice</span><span class="sxs-lookup"><span data-stu-id="55a30-103">Get managedDevice</span></span>

<span data-ttu-id="55a30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55a30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55a30-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55a30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55a30-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55a30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55a30-107">Чтение свойств и связей объекта [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="55a30-107">Read properties and relationships of the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55a30-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55a30-108">Prerequisites</span></span>
<span data-ttu-id="55a30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55a30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55a30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55a30-111">Permission type</span></span>|<span data-ttu-id="55a30-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55a30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55a30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55a30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55a30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55a30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55a30-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55a30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55a30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55a30-116">Not supported.</span></span>|
|<span data-ttu-id="55a30-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55a30-117">Application</span></span>|<span data-ttu-id="55a30-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55a30-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55a30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55a30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55a30-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55a30-120">Optional query parameters</span></span>
<span data-ttu-id="55a30-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55a30-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55a30-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55a30-122">Request headers</span></span>
|<span data-ttu-id="55a30-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55a30-123">Header</span></span>|<span data-ttu-id="55a30-124">Значение</span><span class="sxs-lookup"><span data-stu-id="55a30-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55a30-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55a30-125">Authorization</span></span>|<span data-ttu-id="55a30-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55a30-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55a30-127">Accept</span><span class="sxs-lookup"><span data-stu-id="55a30-127">Accept</span></span>|<span data-ttu-id="55a30-128">application/json</span><span class="sxs-lookup"><span data-stu-id="55a30-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55a30-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55a30-129">Request body</span></span>
<span data-ttu-id="55a30-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55a30-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55a30-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="55a30-131">Response</span></span>
<span data-ttu-id="55a30-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [managedDevice](../resources/intune-shared-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="55a30-132">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55a30-133">Пример</span><span class="sxs-lookup"><span data-stu-id="55a30-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="55a30-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="55a30-134">Request</span></span>
<span data-ttu-id="55a30-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55a30-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="55a30-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="55a30-136">Response</span></span>
<span data-ttu-id="55a30-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55a30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




