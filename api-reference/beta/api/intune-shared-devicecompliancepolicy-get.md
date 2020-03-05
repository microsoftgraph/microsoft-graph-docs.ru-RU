---
title: Get deviceCompliancePolicy
description: Чтение свойств и связей объекта deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d649aaf97ca3785ab54de0a81bb82b6ef69aea36
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458786"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="a2b0d-103">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a2b0d-103">Get deviceCompliancePolicy</span></span>

<span data-ttu-id="a2b0d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2b0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2b0d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2b0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2b0d-107">Чтение свойств и связей объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2b0d-107">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2b0d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a2b0d-108">Prerequisites</span></span>
<span data-ttu-id="a2b0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b0d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2b0d-111">Permission type</span></span>|<span data-ttu-id="a2b0d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2b0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b0d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2b0d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a2b0d-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a2b0d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a2b0d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b0d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a2b0d-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a2b0d-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a2b0d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b0d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2b0d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2b0d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b0d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-119">Not supported.</span></span>|
|<span data-ttu-id="a2b0d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2b0d-120">Application</span></span>|| 
|<span data-ttu-id="a2b0d-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a2b0d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a2b0d-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b0d-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a2b0d-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a2b0d-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a2b0d-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b0d-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b0d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2b0d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2b0d-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2b0d-126">Optional query parameters</span></span>
<span data-ttu-id="a2b0d-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2b0d-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2b0d-128">Request headers</span></span>
|<span data-ttu-id="a2b0d-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2b0d-129">Header</span></span>|<span data-ttu-id="a2b0d-130">Значение</span><span class="sxs-lookup"><span data-stu-id="a2b0d-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2b0d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b0d-131">Authorization</span></span>|<span data-ttu-id="a2b0d-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2b0d-133">Accept</span><span class="sxs-lookup"><span data-stu-id="a2b0d-133">Accept</span></span>|<span data-ttu-id="a2b0d-134">application/json</span><span class="sxs-lookup"><span data-stu-id="a2b0d-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b0d-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2b0d-135">Request body</span></span>
<span data-ttu-id="a2b0d-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2b0d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2b0d-137">Response</span></span>
<span data-ttu-id="a2b0d-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-138">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b0d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a2b0d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2b0d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2b0d-140">Request</span></span>
<span data-ttu-id="a2b0d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a2b0d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2b0d-142">Response</span></span>
<span data-ttu-id="a2b0d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2b0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4214b716-b716-4214-16b7-144216b71442",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```








