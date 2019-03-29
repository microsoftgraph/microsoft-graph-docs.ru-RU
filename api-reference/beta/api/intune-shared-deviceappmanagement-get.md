---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c27099cdc0e2ffbbc3e0e02cde07b9b4e34ea33c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963515"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="a8f30-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a8f30-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="a8f30-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8f30-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8f30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8f30-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8f30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8f30-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a8f30-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8f30-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f30-108">Prerequisites</span></span>

<span data-ttu-id="a8f30-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="a8f30-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a8f30-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f30-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="a8f30-111">Обратите внимание, что соответствующее разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="a8f30-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="a8f30-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f30-112">Permission type</span></span>|<span data-ttu-id="a8f30-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8f30-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="a8f30-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8f30-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="a8f30-115">&nbsp;&nbsp; **Приложения**, **книги**или подключение \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a8f30-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="a8f30-116">DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Реадв. ALL</span><span class="sxs-lookup"><span data-stu-id="a8f30-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="a8f30-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="a8f30-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a8f30-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8f30-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="a8f30-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8f30-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f30-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f30-120">Not supported.</span></span>|
|<span data-ttu-id="a8f30-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8f30-121">Application</span></span>|<span data-ttu-id="a8f30-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f30-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8f30-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8f30-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8f30-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8f30-124">Optional query parameters</span></span>

<span data-ttu-id="a8f30-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8f30-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8f30-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8f30-126">Request headers</span></span>

|<span data-ttu-id="a8f30-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8f30-127">Header</span></span>|<span data-ttu-id="a8f30-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a8f30-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8f30-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8f30-129">Authorization</span></span>|<span data-ttu-id="a8f30-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8f30-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8f30-131">Accept</span><span class="sxs-lookup"><span data-stu-id="a8f30-131">Accept</span></span>|<span data-ttu-id="a8f30-132">application/json</span><span class="sxs-lookup"><span data-stu-id="a8f30-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8f30-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8f30-133">Request body</span></span>

<span data-ttu-id="a8f30-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8f30-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8f30-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8f30-135">Response</span></span>

<span data-ttu-id="a8f30-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a8f30-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8f30-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a8f30-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8f30-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8f30-138">Request</span></span>

<span data-ttu-id="a8f30-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8f30-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="a8f30-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8f30-140">Response</span></span>

<span data-ttu-id="a8f30-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8f30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



