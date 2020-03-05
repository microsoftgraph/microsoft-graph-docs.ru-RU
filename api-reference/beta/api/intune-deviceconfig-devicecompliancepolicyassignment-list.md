---
title: Перечисление объектов deviceCompliancePolicyAssignment
description: Список свойств и связей объектов deviceCompliancePolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6a88d1bbad0da14374ee60aa238c1d7851ff3ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449301"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="45eb4-103">Перечисление объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="45eb4-103">List deviceCompliancePolicyAssignments</span></span>

<span data-ttu-id="45eb4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45eb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45eb4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45eb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45eb4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45eb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45eb4-107">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="45eb4-107">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45eb4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45eb4-108">Prerequisites</span></span>
<span data-ttu-id="45eb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45eb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45eb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45eb4-111">Permission type</span></span>|<span data-ttu-id="45eb4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45eb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45eb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45eb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45eb4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45eb4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45eb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45eb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45eb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45eb4-116">Not supported.</span></span>|
|<span data-ttu-id="45eb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45eb4-117">Application</span></span>|<span data-ttu-id="45eb4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45eb4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45eb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45eb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="45eb4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45eb4-120">Request headers</span></span>
|<span data-ttu-id="45eb4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45eb4-121">Header</span></span>|<span data-ttu-id="45eb4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45eb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45eb4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45eb4-123">Authorization</span></span>|<span data-ttu-id="45eb4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45eb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45eb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45eb4-125">Accept</span></span>|<span data-ttu-id="45eb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45eb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45eb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45eb4-127">Request body</span></span>
<span data-ttu-id="45eb4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45eb4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45eb4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="45eb4-129">Response</span></span>
<span data-ttu-id="45eb4-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45eb4-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45eb4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="45eb4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45eb4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45eb4-132">Request</span></span>
<span data-ttu-id="45eb4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45eb4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="45eb4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="45eb4-134">Response</span></span>
<span data-ttu-id="45eb4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45eb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 343

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```





