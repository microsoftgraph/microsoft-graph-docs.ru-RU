---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 798fa1eb36a9f9dd58aae6cae8dd4e4960b6299c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864617"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="83807-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="83807-103">Get deviceAppManagement</span></span>

<span data-ttu-id="83807-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83807-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83807-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="83807-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83807-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83807-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83807-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83807-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83807-108">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="83807-108">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83807-109">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="83807-109">Prerequisites</span></span>

<span data-ttu-id="83807-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="83807-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="83807-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83807-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="83807-112">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="83807-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="83807-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83807-113">Permission type</span></span>|<span data-ttu-id="83807-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83807-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="83807-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83807-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="83807-116">&nbsp;&nbsp; **Приложения,** **книги,** **onboarding,** **интеграция партнеров** или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="83807-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="83807-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="83807-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="83807-118">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="83807-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="83807-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="83807-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="83807-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83807-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83807-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83807-121">Not supported.</span></span>|
|<span data-ttu-id="83807-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="83807-122">Application</span></span>| |
| <span data-ttu-id="83807-123">&nbsp;&nbsp; **Приложения,** **книги,** **onboarding,** **интеграция партнеров** или **набор политик**</span><span class="sxs-lookup"><span data-stu-id="83807-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="83807-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="83807-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="83807-125">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="83807-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="83807-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="83807-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83807-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83807-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83807-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="83807-128">Optional query parameters</span></span>

<span data-ttu-id="83807-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="83807-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83807-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83807-130">Request headers</span></span>

|<span data-ttu-id="83807-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83807-131">Header</span></span>|<span data-ttu-id="83807-132">Значение</span><span class="sxs-lookup"><span data-stu-id="83807-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83807-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83807-133">Authorization</span></span>|<span data-ttu-id="83807-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83807-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83807-135">Accept</span><span class="sxs-lookup"><span data-stu-id="83807-135">Accept</span></span>|<span data-ttu-id="83807-136">application/json</span><span class="sxs-lookup"><span data-stu-id="83807-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83807-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83807-137">Request body</span></span>

<span data-ttu-id="83807-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83807-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83807-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="83807-139">Response</span></span>

<span data-ttu-id="83807-140">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="83807-140">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83807-141">Пример</span><span class="sxs-lookup"><span data-stu-id="83807-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="83807-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="83807-142">Request</span></span>

<span data-ttu-id="83807-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83807-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="83807-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="83807-144">Response</span></span>

<span data-ttu-id="83807-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83807-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










