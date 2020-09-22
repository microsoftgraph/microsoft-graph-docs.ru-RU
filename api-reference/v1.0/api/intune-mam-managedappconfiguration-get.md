---
title: Get managedAppConfiguration
description: Чтение свойств и связей объекта managedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cf54fdfc34ce9541ac355dbf553aac93cff9091
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015913"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="71adf-103">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="71adf-103">Get managedAppConfiguration</span></span>

<span data-ttu-id="71adf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71adf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71adf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71adf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71adf-106">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71adf-106">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71adf-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="71adf-107">Prerequisites</span></span>
<span data-ttu-id="71adf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71adf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71adf-110">Permission type</span></span>|<span data-ttu-id="71adf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71adf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71adf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71adf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71adf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="71adf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="71adf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71adf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71adf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71adf-115">Not supported.</span></span>|
|<span data-ttu-id="71adf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71adf-116">Application</span></span>|<span data-ttu-id="71adf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71adf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71adf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71adf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71adf-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="71adf-119">Optional query parameters</span></span>
<span data-ttu-id="71adf-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71adf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71adf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71adf-121">Request headers</span></span>
|<span data-ttu-id="71adf-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71adf-122">Header</span></span>|<span data-ttu-id="71adf-123">Значение</span><span class="sxs-lookup"><span data-stu-id="71adf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71adf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71adf-124">Authorization</span></span>|<span data-ttu-id="71adf-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71adf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71adf-126">Accept</span><span class="sxs-lookup"><span data-stu-id="71adf-126">Accept</span></span>|<span data-ttu-id="71adf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="71adf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71adf-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71adf-128">Request body</span></span>
<span data-ttu-id="71adf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71adf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71adf-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="71adf-130">Response</span></span>
<span data-ttu-id="71adf-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71adf-131">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71adf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="71adf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="71adf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="71adf-133">Request</span></span>
<span data-ttu-id="71adf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71adf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="71adf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="71adf-135">Response</span></span>
<span data-ttu-id="71adf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71adf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```









