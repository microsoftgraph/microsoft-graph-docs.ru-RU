---
title: Получение Девицеманажементскриптграупассигнмент
description: Чтение свойств и связей объекта Девицеманажементскриптграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c2edc45405a3a7146da68a7126ec74c35c44592
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087526"
---
# <a name="get-devicemanagementscriptgroupassignment"></a><span data-ttu-id="22883-103">Получение Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="22883-103">Get deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="22883-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22883-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22883-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22883-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22883-106">Чтение свойств и связей объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="22883-106">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22883-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22883-107">Prerequisites</span></span>
<span data-ttu-id="22883-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22883-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22883-110">Permission type</span></span>|<span data-ttu-id="22883-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22883-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22883-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22883-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22883-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="22883-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="22883-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22883-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22883-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22883-115">Not supported.</span></span>|
|<span data-ttu-id="22883-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22883-116">Application</span></span>|<span data-ttu-id="22883-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="22883-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22883-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22883-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22883-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22883-119">Optional query parameters</span></span>
<span data-ttu-id="22883-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22883-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22883-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22883-121">Request headers</span></span>
|<span data-ttu-id="22883-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22883-122">Header</span></span>|<span data-ttu-id="22883-123">Значение</span><span class="sxs-lookup"><span data-stu-id="22883-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22883-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22883-124">Authorization</span></span>|<span data-ttu-id="22883-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22883-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22883-126">Accept</span><span class="sxs-lookup"><span data-stu-id="22883-126">Accept</span></span>|<span data-ttu-id="22883-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22883-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22883-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22883-128">Request body</span></span>
<span data-ttu-id="22883-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22883-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22883-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="22883-130">Response</span></span>
<span data-ttu-id="22883-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22883-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22883-132">Пример</span><span class="sxs-lookup"><span data-stu-id="22883-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22883-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="22883-133">Request</span></span>
<span data-ttu-id="22883-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22883-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="22883-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="22883-135">Response</span></span>
<span data-ttu-id="22883-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22883-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 198

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
    "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
    "targetGroupId": "Target Group Id value"
  }
}
```






