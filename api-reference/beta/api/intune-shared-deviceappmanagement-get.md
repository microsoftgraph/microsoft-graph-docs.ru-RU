---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6a6e8e58167cd9471802be39f9e7d6c1744040e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350995"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="12152-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="12152-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="12152-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12152-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12152-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12152-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12152-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12152-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12152-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="12152-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12152-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="12152-108">Prerequisites</span></span>

<span data-ttu-id="12152-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="12152-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="12152-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12152-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="12152-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="12152-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="12152-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12152-112">Permission type</span></span>|<span data-ttu-id="12152-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12152-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="12152-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12152-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="12152-115">&nbsp;&nbsp; **Приложения**, **книги**, входящая миграция или **Интеграция партнерских** **систем**</span><span class="sxs-lookup"><span data-stu-id="12152-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, or **Partner Integration**</span></span> | <span data-ttu-id="12152-116">DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Реадв. ALL</span><span class="sxs-lookup"><span data-stu-id="12152-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="12152-117">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="12152-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="12152-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="12152-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="12152-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12152-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12152-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12152-120">Not supported.</span></span>|
|<span data-ttu-id="12152-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12152-121">Application</span></span>|<span data-ttu-id="12152-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12152-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12152-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12152-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12152-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12152-124">Optional query parameters</span></span>

<span data-ttu-id="12152-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12152-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12152-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12152-126">Request headers</span></span>

|<span data-ttu-id="12152-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12152-127">Header</span></span>|<span data-ttu-id="12152-128">Значение</span><span class="sxs-lookup"><span data-stu-id="12152-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12152-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12152-129">Authorization</span></span>|<span data-ttu-id="12152-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12152-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12152-131">Accept</span><span class="sxs-lookup"><span data-stu-id="12152-131">Accept</span></span>|<span data-ttu-id="12152-132">application/json</span><span class="sxs-lookup"><span data-stu-id="12152-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12152-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12152-133">Request body</span></span>

<span data-ttu-id="12152-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12152-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12152-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="12152-135">Response</span></span>

<span data-ttu-id="12152-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12152-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12152-137">Пример</span><span class="sxs-lookup"><span data-stu-id="12152-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="12152-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="12152-138">Request</span></span>

<span data-ttu-id="12152-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12152-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="12152-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="12152-140">Response</span></span>

<span data-ttu-id="12152-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12152-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






