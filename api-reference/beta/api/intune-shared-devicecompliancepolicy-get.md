---
title: Get deviceCompliancePolicy
description: Чтение свойств и связей объекта deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e401e2b4ae6e476a507ec4ec20d13248a909cd4d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940126"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="cf016-103">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cf016-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="cf016-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf016-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf016-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf016-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf016-106">Чтение свойств и связей объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf016-106">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf016-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cf016-107">Prerequisites</span></span>
<span data-ttu-id="cf016-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf016-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf016-110">Permission type</span></span>|<span data-ttu-id="cf016-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf016-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf016-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf016-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cf016-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="cf016-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cf016-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf016-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="cf016-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="cf016-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cf016-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf016-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf016-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf016-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf016-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf016-118">Not supported.</span></span>|
|<span data-ttu-id="cf016-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf016-119">Application</span></span>|| 
|<span data-ttu-id="cf016-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="cf016-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cf016-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf016-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="cf016-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="cf016-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cf016-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf016-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf016-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf016-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf016-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf016-125">Optional query parameters</span></span>
<span data-ttu-id="cf016-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf016-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf016-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf016-127">Request headers</span></span>
|<span data-ttu-id="cf016-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf016-128">Header</span></span>|<span data-ttu-id="cf016-129">Значение</span><span class="sxs-lookup"><span data-stu-id="cf016-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf016-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf016-130">Authorization</span></span>|<span data-ttu-id="cf016-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf016-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf016-132">Accept</span><span class="sxs-lookup"><span data-stu-id="cf016-132">Accept</span></span>|<span data-ttu-id="cf016-133">application/json</span><span class="sxs-lookup"><span data-stu-id="cf016-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf016-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf016-134">Request body</span></span>
<span data-ttu-id="cf016-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf016-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf016-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf016-136">Response</span></span>
<span data-ttu-id="cf016-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cf016-137">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf016-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cf016-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf016-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf016-139">Request</span></span>
<span data-ttu-id="cf016-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf016-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="cf016-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf016-141">Response</span></span>
<span data-ttu-id="cf016-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf016-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








