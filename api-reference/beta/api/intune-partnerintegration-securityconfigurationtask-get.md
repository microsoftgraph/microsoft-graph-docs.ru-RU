---
title: Получить securityConfigurationTask
description: Чтение свойств и связей объекта securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7146f9aed80574a38f9d76e2b0048759cd6be2e7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134818"
---
# <a name="get-securityconfigurationtask"></a><span data-ttu-id="ed524-103">Получить securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="ed524-103">Get securityConfigurationTask</span></span>

<span data-ttu-id="ed524-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed524-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed524-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed524-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed524-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed524-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed524-107">Чтение свойств и связей объекта [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)</span><span class="sxs-lookup"><span data-stu-id="ed524-107">Read properties and relationships of the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed524-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed524-108">Prerequisites</span></span>
<span data-ttu-id="ed524-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed524-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed524-111">Permission type</span></span>|<span data-ttu-id="ed524-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed524-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed524-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed524-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed524-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed524-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed524-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed524-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed524-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed524-116">Not supported.</span></span>|
|<span data-ttu-id="ed524-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ed524-117">Application</span></span>|<span data-ttu-id="ed524-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed524-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed524-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed524-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed524-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ed524-120">Optional query parameters</span></span>
<span data-ttu-id="ed524-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ed524-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed524-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed524-122">Request headers</span></span>
|<span data-ttu-id="ed524-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed524-123">Header</span></span>|<span data-ttu-id="ed524-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ed524-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed524-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed524-125">Authorization</span></span>|<span data-ttu-id="ed524-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed524-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed524-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ed524-127">Accept</span></span>|<span data-ttu-id="ed524-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ed524-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed524-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed524-129">Request body</span></span>
<span data-ttu-id="ed524-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed524-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed524-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed524-131">Response</span></span>
<span data-ttu-id="ed524-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ed524-132">If successful, this method returns a `200 OK` response code and [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed524-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ed524-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed524-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed524-134">Request</span></span>
<span data-ttu-id="ed524-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed524-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

### <a name="response"></a><span data-ttu-id="ed524-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed524-136">Response</span></span>
<span data-ttu-id="ed524-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed524-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 921

{
  "value": {
    "@odata.type": "#microsoft.graph.securityConfigurationTask",
    "id": "5d630f12-0f12-5d63-120f-635d120f635d",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
    "category": "advancedThreatProtection",
    "priority": "high",
    "creator": "Creator value",
    "creatorNotes": "Creator Notes value",
    "assignedTo": "Assigned To value",
    "status": "pending",
    "endpointSecurityPolicy": "antivirus",
    "applicablePlatform": "macOS",
    "endpointSecurityPolicyProfile": "antivirus",
    "insights": "Insights value",
    "managedDeviceCount": 2,
    "intendedSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```




