---
title: Get deviceCompliancePolicyAssignment
description: Чтение свойств и связей объекта deviceCompliancePolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5b71651e3edde8099759612519ac79319af71ae
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755800"
---
# <a name="get-devicecompliancepolicyassignment"></a><span data-ttu-id="174a0-103">Get deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="174a0-103">Get deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="174a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="174a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="174a0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="174a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="174a0-106">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="174a0-106">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="174a0-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="174a0-107">Prerequisites</span></span>
<span data-ttu-id="174a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="174a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="174a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="174a0-110">Permission type</span></span>|<span data-ttu-id="174a0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="174a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="174a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="174a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="174a0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="174a0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="174a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="174a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="174a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="174a0-115">Not supported.</span></span>|
|<span data-ttu-id="174a0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="174a0-116">Application</span></span>|<span data-ttu-id="174a0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="174a0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="174a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="174a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="174a0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="174a0-119">Optional query parameters</span></span>
<span data-ttu-id="174a0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="174a0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="174a0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="174a0-121">Request headers</span></span>
|<span data-ttu-id="174a0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="174a0-122">Header</span></span>|<span data-ttu-id="174a0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="174a0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="174a0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="174a0-124">Authorization</span></span>|<span data-ttu-id="174a0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="174a0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="174a0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="174a0-126">Accept</span></span>|<span data-ttu-id="174a0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="174a0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="174a0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="174a0-128">Request body</span></span>
<span data-ttu-id="174a0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="174a0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="174a0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="174a0-130">Response</span></span>
<span data-ttu-id="174a0-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="174a0-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="174a0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="174a0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="174a0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="174a0-133">Request</span></span>
<span data-ttu-id="174a0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="174a0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="174a0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="174a0-135">Response</span></span>
<span data-ttu-id="174a0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="174a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
    "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```




