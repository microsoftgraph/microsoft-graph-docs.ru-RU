---
title: Get deviceCompliancePolicy
description: Чтение свойств и связей объекта deviceCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b22ac4c5b1f4fb8affdbf89ad08af6223472bab
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801210"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="b9f15-103">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b9f15-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="b9f15-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f15-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9f15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f15-106">Чтение свойств и связей объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b9f15-106">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9f15-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f15-107">Prerequisites</span></span>
<span data-ttu-id="b9f15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f15-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f15-110">Permission type</span></span>|<span data-ttu-id="b9f15-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f15-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f15-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b9f15-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="b9f15-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b9f15-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f15-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b9f15-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b9f15-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b9f15-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f15-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9f15-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f15-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f15-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f15-118">Not supported.</span></span>|
|<span data-ttu-id="b9f15-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9f15-119">Application</span></span>|| 
|<span data-ttu-id="b9f15-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="b9f15-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b9f15-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f15-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b9f15-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b9f15-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b9f15-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f15-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f15-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f15-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9f15-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9f15-125">Optional query parameters</span></span>
<span data-ttu-id="b9f15-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f15-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9f15-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f15-127">Request headers</span></span>
|<span data-ttu-id="b9f15-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9f15-128">Header</span></span>|<span data-ttu-id="b9f15-129">Значение</span><span class="sxs-lookup"><span data-stu-id="b9f15-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f15-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f15-130">Authorization</span></span>|<span data-ttu-id="b9f15-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9f15-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f15-132">Accept</span><span class="sxs-lookup"><span data-stu-id="b9f15-132">Accept</span></span>|<span data-ttu-id="b9f15-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f15-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f15-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9f15-134">Request body</span></span>
<span data-ttu-id="b9f15-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9f15-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f15-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9f15-136">Response</span></span>
<span data-ttu-id="b9f15-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f15-137">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f15-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b9f15-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9f15-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f15-139">Request</span></span>
<span data-ttu-id="b9f15-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9f15-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="b9f15-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f15-141">Response</span></span>
<span data-ttu-id="b9f15-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9f15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







