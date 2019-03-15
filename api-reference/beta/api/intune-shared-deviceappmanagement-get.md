---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7a7bc478dc4a9a59b067b5acb3688c0bb0793d9f
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570824"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="94862-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="94862-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="94862-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94862-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94862-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94862-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94862-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94862-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="94862-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94862-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="94862-108">Prerequisites</span></span>

<span data-ttu-id="94862-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="94862-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="94862-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="94862-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>  <span data-ttu-id="94862-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="94862-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="94862-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94862-112">Permission type</span></span>|<span data-ttu-id="94862-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94862-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="94862-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94862-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="94862-115">&nbsp;&nbsp; **Приложения**, **книги**или подключение \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="94862-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="94862-116">DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Реадв. ALL</span><span class="sxs-lookup"><span data-stu-id="94862-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="94862-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="94862-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="94862-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="94862-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="94862-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94862-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94862-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94862-120">Not supported.</span></span>|
|<span data-ttu-id="94862-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94862-121">Application</span></span>|<span data-ttu-id="94862-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94862-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94862-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94862-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94862-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94862-124">Optional query parameters</span></span>

<span data-ttu-id="94862-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94862-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94862-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94862-126">Request headers</span></span>

|<span data-ttu-id="94862-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94862-127">Header</span></span>|<span data-ttu-id="94862-128">Значение</span><span class="sxs-lookup"><span data-stu-id="94862-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94862-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94862-129">Authorization</span></span>|<span data-ttu-id="94862-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94862-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94862-131">Accept</span><span class="sxs-lookup"><span data-stu-id="94862-131">Accept</span></span>|<span data-ttu-id="94862-132">application/json</span><span class="sxs-lookup"><span data-stu-id="94862-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94862-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94862-133">Request body</span></span>

<span data-ttu-id="94862-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94862-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94862-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="94862-135">Response</span></span>

<span data-ttu-id="94862-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="94862-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94862-137">Пример</span><span class="sxs-lookup"><span data-stu-id="94862-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="94862-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="94862-138">Request</span></span>

<span data-ttu-id="94862-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94862-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="94862-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="94862-140">Response</span></span>

<span data-ttu-id="94862-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94862-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



