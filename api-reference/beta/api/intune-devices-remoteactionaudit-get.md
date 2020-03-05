---
title: Получение remoteActionAudit
description: Чтение свойств и связей объекта remoteActionAudit.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ead3b301285f40aaa1ab7315b4587d00d88857c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468623"
---
# <a name="get-remoteactionaudit"></a><span data-ttu-id="5b350-103">Получение remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="5b350-103">Get remoteActionAudit</span></span>

<span data-ttu-id="5b350-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5b350-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b350-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b350-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b350-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b350-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b350-107">Чтение свойств и связей объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="5b350-107">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b350-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b350-108">Prerequisites</span></span>
<span data-ttu-id="5b350-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b350-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b350-111">Permission type</span></span>|<span data-ttu-id="5b350-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b350-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b350-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b350-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b350-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b350-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5b350-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b350-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b350-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b350-116">Not supported.</span></span>|
|<span data-ttu-id="5b350-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b350-117">Application</span></span>|<span data-ttu-id="5b350-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b350-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b350-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b350-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b350-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b350-120">Optional query parameters</span></span>
<span data-ttu-id="5b350-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b350-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b350-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b350-122">Request headers</span></span>
|<span data-ttu-id="5b350-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b350-123">Header</span></span>|<span data-ttu-id="5b350-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5b350-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b350-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b350-125">Authorization</span></span>|<span data-ttu-id="5b350-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b350-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b350-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5b350-127">Accept</span></span>|<span data-ttu-id="5b350-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b350-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b350-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b350-129">Request body</span></span>
<span data-ttu-id="5b350-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b350-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b350-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b350-131">Response</span></span>
<span data-ttu-id="5b350-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b350-132">If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b350-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5b350-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b350-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b350-134">Request</span></span>
<span data-ttu-id="5b350-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b350-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="5b350-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b350-136">Response</span></span>
<span data-ttu-id="5b350-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b350-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





