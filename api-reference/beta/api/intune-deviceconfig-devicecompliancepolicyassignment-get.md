---
title: Get deviceCompliancePolicyAssignment
description: Чтение свойств и связей объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 568142105e6a22dceb7c2da9636eeb6f9ef91813
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735017"
---
# <a name="get-devicecompliancepolicyassignment"></a><span data-ttu-id="a46e7-103">Get deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a46e7-103">Get deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="a46e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a46e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a46e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a46e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a46e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a46e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a46e7-107">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a46e7-107">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a46e7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a46e7-108">Prerequisites</span></span>
<span data-ttu-id="a46e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a46e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a46e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a46e7-111">Permission type</span></span>|<span data-ttu-id="a46e7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a46e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a46e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a46e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a46e7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a46e7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a46e7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a46e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a46e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a46e7-116">Not supported.</span></span>|
|<span data-ttu-id="a46e7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a46e7-117">Application</span></span>|<span data-ttu-id="a46e7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a46e7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a46e7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a46e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a46e7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a46e7-120">Optional query parameters</span></span>
<span data-ttu-id="a46e7-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a46e7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a46e7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a46e7-122">Request headers</span></span>
|<span data-ttu-id="a46e7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a46e7-123">Header</span></span>|<span data-ttu-id="a46e7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a46e7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a46e7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a46e7-125">Authorization</span></span>|<span data-ttu-id="a46e7-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a46e7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a46e7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a46e7-127">Accept</span></span>|<span data-ttu-id="a46e7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a46e7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a46e7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a46e7-129">Request body</span></span>
<span data-ttu-id="a46e7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a46e7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a46e7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a46e7-131">Response</span></span>
<span data-ttu-id="a46e7-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a46e7-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a46e7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a46e7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a46e7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a46e7-134">Request</span></span>
<span data-ttu-id="a46e7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a46e7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a46e7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a46e7-136">Response</span></span>
<span data-ttu-id="a46e7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a46e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
    "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```





