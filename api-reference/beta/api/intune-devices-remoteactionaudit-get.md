---
title: Get remoteActionAudit
description: Чтение свойств и связей объекта remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17968a28a43bdda04ce6f2150629eac2d995f0cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158215"
---
# <a name="get-remoteactionaudit"></a><span data-ttu-id="d4efb-103">Get remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d4efb-103">Get remoteActionAudit</span></span>

<span data-ttu-id="d4efb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4efb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4efb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4efb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4efb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4efb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4efb-107">Чтение свойств и связей объекта [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="d4efb-107">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4efb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4efb-108">Prerequisites</span></span>
<span data-ttu-id="d4efb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4efb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4efb-111">Permission type</span></span>|<span data-ttu-id="d4efb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4efb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4efb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4efb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4efb-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4efb-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d4efb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4efb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4efb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4efb-116">Not supported.</span></span>|
|<span data-ttu-id="d4efb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4efb-117">Application</span></span>|<span data-ttu-id="d4efb-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4efb-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4efb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4efb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4efb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4efb-120">Optional query parameters</span></span>
<span data-ttu-id="d4efb-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d4efb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4efb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4efb-122">Request headers</span></span>
|<span data-ttu-id="d4efb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4efb-123">Header</span></span>|<span data-ttu-id="d4efb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d4efb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4efb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4efb-125">Authorization</span></span>|<span data-ttu-id="d4efb-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4efb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4efb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d4efb-127">Accept</span></span>|<span data-ttu-id="d4efb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d4efb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4efb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4efb-129">Request body</span></span>
<span data-ttu-id="d4efb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4efb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4efb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4efb-131">Response</span></span>
<span data-ttu-id="d4efb-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4efb-132">If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4efb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d4efb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4efb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4efb-134">Request</span></span>
<span data-ttu-id="d4efb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4efb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="d4efb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4efb-136">Response</span></span>
<span data-ttu-id="d4efb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4efb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteActionAudit",
    "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "action": "factoryReset",
    "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
    "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
    "deviceIMEI": "Device IMEI value",
    "actionState": "pending",
    "managedDeviceId": "Managed Device Id value"
  }
}
```




