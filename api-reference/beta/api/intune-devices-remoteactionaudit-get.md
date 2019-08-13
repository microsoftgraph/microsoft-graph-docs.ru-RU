---
title: Получение remoteActionAudit
description: Чтение свойств и связей объекта remoteActionAudit.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ec834c6762daf6ba2317d3a5fc12c87c8f3cb97
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310012"
---
# <a name="get-remoteactionaudit"></a><span data-ttu-id="54132-103">Получение remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="54132-103">Get remoteActionAudit</span></span>

> <span data-ttu-id="54132-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54132-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54132-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54132-106">Чтение свойств и связей объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="54132-106">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54132-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="54132-107">Prerequisites</span></span>
<span data-ttu-id="54132-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54132-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54132-110">Permission type</span></span>|<span data-ttu-id="54132-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54132-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54132-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54132-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54132-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="54132-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="54132-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54132-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54132-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54132-115">Not supported.</span></span>|
|<span data-ttu-id="54132-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54132-116">Application</span></span>|<span data-ttu-id="54132-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="54132-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54132-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54132-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54132-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54132-119">Optional query parameters</span></span>
<span data-ttu-id="54132-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="54132-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54132-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54132-121">Request headers</span></span>
|<span data-ttu-id="54132-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54132-122">Header</span></span>|<span data-ttu-id="54132-123">Значение</span><span class="sxs-lookup"><span data-stu-id="54132-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54132-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54132-124">Authorization</span></span>|<span data-ttu-id="54132-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54132-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54132-126">Accept</span><span class="sxs-lookup"><span data-stu-id="54132-126">Accept</span></span>|<span data-ttu-id="54132-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54132-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54132-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54132-128">Request body</span></span>
<span data-ttu-id="54132-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54132-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54132-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="54132-130">Response</span></span>
<span data-ttu-id="54132-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54132-131">If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54132-132">Пример</span><span class="sxs-lookup"><span data-stu-id="54132-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="54132-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="54132-133">Request</span></span>
<span data-ttu-id="54132-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54132-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="54132-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="54132-135">Response</span></span>
<span data-ttu-id="54132-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54132-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






