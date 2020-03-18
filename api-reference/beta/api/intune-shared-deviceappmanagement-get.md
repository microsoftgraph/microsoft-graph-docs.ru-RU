---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2bb20886dc19e3a1faca1ca7bd7bb640ec43f6cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801273"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="f511c-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="f511c-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="f511c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f511c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f511c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f511c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f511c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f511c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f511c-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f511c-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f511c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f511c-108">Prerequisites</span></span>

<span data-ttu-id="f511c-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="f511c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f511c-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f511c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f511c-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="f511c-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="f511c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f511c-112">Permission type</span></span>|<span data-ttu-id="f511c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f511c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="f511c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f511c-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="f511c-115">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="f511c-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="f511c-116">DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Реадв. ALL</span><span class="sxs-lookup"><span data-stu-id="f511c-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="f511c-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f511c-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f511c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f511c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="f511c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f511c-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f511c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f511c-120">Not supported.</span></span>|
|<span data-ttu-id="f511c-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="f511c-121">Application</span></span>| |
| <span data-ttu-id="f511c-122">&nbsp;&nbsp; **Приложения**, **книги**, **входящая**миграция, **Интеграция партнеров**или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="f511c-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="f511c-123">DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Реадв. ALL</span><span class="sxs-lookup"><span data-stu-id="f511c-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="f511c-124">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f511c-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f511c-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f511c-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f511c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f511c-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f511c-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f511c-127">Optional query parameters</span></span>

<span data-ttu-id="f511c-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f511c-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f511c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f511c-129">Request headers</span></span>

|<span data-ttu-id="f511c-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f511c-130">Header</span></span>|<span data-ttu-id="f511c-131">Значение</span><span class="sxs-lookup"><span data-stu-id="f511c-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f511c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f511c-132">Authorization</span></span>|<span data-ttu-id="f511c-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f511c-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f511c-134">Accept</span><span class="sxs-lookup"><span data-stu-id="f511c-134">Accept</span></span>|<span data-ttu-id="f511c-135">application/json</span><span class="sxs-lookup"><span data-stu-id="f511c-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f511c-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f511c-136">Request body</span></span>

<span data-ttu-id="f511c-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f511c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f511c-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f511c-138">Response</span></span>

<span data-ttu-id="f511c-139">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f511c-139">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f511c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f511c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f511c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f511c-141">Request</span></span>

<span data-ttu-id="f511c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f511c-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="f511c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f511c-143">Response</span></span>

<span data-ttu-id="f511c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f511c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










