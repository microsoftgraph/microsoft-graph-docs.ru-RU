---
title: Список Ремотеактионаудитс
description: Список свойств и связей объектов remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da671f30f18ddda7f71e92f94c6d3709f77cc307
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212743"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="ca9e7-103">Список Ремотеактионаудитс</span><span class="sxs-lookup"><span data-stu-id="ca9e7-103">List remoteActionAudits</span></span>

<span data-ttu-id="ca9e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca9e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca9e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca9e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9e7-107">Список свойств и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="ca9e7-107">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca9e7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca9e7-108">Prerequisites</span></span>
<span data-ttu-id="ca9e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca9e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca9e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca9e7-111">Permission type</span></span>|<span data-ttu-id="ca9e7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca9e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca9e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca9e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca9e7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca9e7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ca9e7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca9e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca9e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-116">Not supported.</span></span>|
|<span data-ttu-id="ca9e7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca9e7-117">Application</span></span>|<span data-ttu-id="ca9e7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca9e7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca9e7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca9e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="ca9e7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ca9e7-120">Request headers</span></span>
|<span data-ttu-id="ca9e7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca9e7-121">Header</span></span>|<span data-ttu-id="ca9e7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca9e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca9e7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca9e7-123">Authorization</span></span>|<span data-ttu-id="ca9e7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca9e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca9e7-125">Accept</span></span>|<span data-ttu-id="ca9e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca9e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca9e7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca9e7-127">Request body</span></span>
<span data-ttu-id="ca9e7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca9e7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca9e7-129">Response</span></span>
<span data-ttu-id="ca9e7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-130">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca9e7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ca9e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca9e7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca9e7-132">Request</span></span>
<span data-ttu-id="ca9e7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="ca9e7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca9e7-134">Response</span></span>
<span data-ttu-id="ca9e7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca9e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": [
    {
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
  ]
}
```




