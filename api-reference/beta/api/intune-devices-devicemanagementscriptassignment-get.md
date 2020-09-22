---
title: Получение Девицеманажементскриптассигнмент
description: Чтение свойств и связей объекта Девицеманажементскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bad3c3fd33d6686ca2b6d337195e74ce0c77c082
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056095"
---
# <a name="get-devicemanagementscriptassignment"></a><span data-ttu-id="0afd9-103">Получение Девицеманажементскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="0afd9-103">Get deviceManagementScriptAssignment</span></span>

<span data-ttu-id="0afd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0afd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0afd9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0afd9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0afd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0afd9-107">Чтение свойств и связей объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="0afd9-107">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0afd9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0afd9-108">Prerequisites</span></span>
<span data-ttu-id="0afd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0afd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0afd9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0afd9-111">Permission type</span></span>|<span data-ttu-id="0afd9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0afd9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0afd9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0afd9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0afd9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0afd9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0afd9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0afd9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0afd9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd9-116">Not supported.</span></span>|
|<span data-ttu-id="0afd9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0afd9-117">Application</span></span>|<span data-ttu-id="0afd9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0afd9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0afd9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0afd9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0afd9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0afd9-120">Optional query parameters</span></span>
<span data-ttu-id="0afd9-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0afd9-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0afd9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0afd9-122">Request headers</span></span>
|<span data-ttu-id="0afd9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0afd9-123">Header</span></span>|<span data-ttu-id="0afd9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0afd9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0afd9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0afd9-125">Authorization</span></span>|<span data-ttu-id="0afd9-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0afd9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0afd9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0afd9-127">Accept</span></span>|<span data-ttu-id="0afd9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0afd9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0afd9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0afd9-129">Request body</span></span>
<span data-ttu-id="0afd9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0afd9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0afd9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0afd9-131">Response</span></span>
<span data-ttu-id="0afd9-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0afd9-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0afd9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0afd9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0afd9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0afd9-134">Request</span></span>
<span data-ttu-id="0afd9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0afd9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0afd9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0afd9-136">Response</span></span>
<span data-ttu-id="0afd9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0afd9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
    "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```






