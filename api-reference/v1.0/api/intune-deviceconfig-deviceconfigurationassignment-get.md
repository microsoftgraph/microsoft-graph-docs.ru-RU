---
title: Get deviceConfigurationAssignment
description: Чтение свойств и связей объекта deviceConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9112fe00cce1fad641d2f6c62057ce9c74605a21
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514826"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="d94b4-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d94b4-103">Get deviceConfigurationAssignment</span></span>

<span data-ttu-id="d94b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d94b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d94b4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d94b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d94b4-106">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d94b4-106">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d94b4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d94b4-107">Prerequisites</span></span>
<span data-ttu-id="d94b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d94b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d94b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d94b4-110">Permission type</span></span>|<span data-ttu-id="d94b4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d94b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d94b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d94b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d94b4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d94b4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d94b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d94b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d94b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d94b4-115">Not supported.</span></span>|
|<span data-ttu-id="d94b4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d94b4-116">Application</span></span>|<span data-ttu-id="d94b4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d94b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d94b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d94b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d94b4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d94b4-119">Optional query parameters</span></span>
<span data-ttu-id="d94b4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d94b4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d94b4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d94b4-121">Request headers</span></span>
|<span data-ttu-id="d94b4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d94b4-122">Header</span></span>|<span data-ttu-id="d94b4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d94b4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d94b4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d94b4-124">Authorization</span></span>|<span data-ttu-id="d94b4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d94b4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d94b4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d94b4-126">Accept</span></span>|<span data-ttu-id="d94b4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d94b4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d94b4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d94b4-128">Request body</span></span>
<span data-ttu-id="d94b4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d94b4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d94b4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d94b4-130">Response</span></span>
<span data-ttu-id="d94b4-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d94b4-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d94b4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d94b4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d94b4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d94b4-133">Request</span></span>
<span data-ttu-id="d94b4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d94b4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d94b4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d94b4-135">Response</span></span>
<span data-ttu-id="d94b4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d94b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




