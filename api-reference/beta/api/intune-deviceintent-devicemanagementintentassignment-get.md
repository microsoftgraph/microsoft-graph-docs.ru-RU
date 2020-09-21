---
title: Получение Девицеманажементинтентассигнмент
description: Чтение свойств и связей объекта Девицеманажементинтентассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df5aa1a73d837a6f963bf5afa4400e4258b4964a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054450"
---
# <a name="get-devicemanagementintentassignment"></a><span data-ttu-id="e2861-103">Получение Девицеманажементинтентассигнмент</span><span class="sxs-lookup"><span data-stu-id="e2861-103">Get deviceManagementIntentAssignment</span></span>

<span data-ttu-id="e2861-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2861-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2861-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2861-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2861-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2861-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2861-107">Чтение свойств и связей объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e2861-107">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2861-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2861-108">Prerequisites</span></span>
<span data-ttu-id="e2861-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2861-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2861-111">Permission type</span></span>|<span data-ttu-id="e2861-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2861-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2861-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2861-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2861-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2861-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e2861-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2861-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2861-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2861-116">Not supported.</span></span>|
|<span data-ttu-id="e2861-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2861-117">Application</span></span>|<span data-ttu-id="e2861-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2861-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2861-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2861-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2861-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2861-120">Optional query parameters</span></span>
<span data-ttu-id="e2861-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2861-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2861-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2861-122">Request headers</span></span>
|<span data-ttu-id="e2861-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2861-123">Header</span></span>|<span data-ttu-id="e2861-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e2861-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2861-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2861-125">Authorization</span></span>|<span data-ttu-id="e2861-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2861-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2861-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e2861-127">Accept</span></span>|<span data-ttu-id="e2861-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2861-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2861-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2861-129">Request body</span></span>
<span data-ttu-id="e2861-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2861-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2861-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2861-131">Response</span></span>
<span data-ttu-id="e2861-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2861-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2861-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e2861-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2861-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2861-134">Request</span></span>
<span data-ttu-id="e2861-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2861-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e2861-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2861-136">Response</span></span>
<span data-ttu-id="e2861-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2861-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
    "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```






