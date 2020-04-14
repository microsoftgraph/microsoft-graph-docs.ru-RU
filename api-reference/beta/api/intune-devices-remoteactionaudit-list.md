---
title: Список Ремотеактионаудитс
description: Список свойств и связей объектов remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b3f3ada26bdc666568ab6e1c7ad8312493d4cea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43323584"
---
# <a name="list-remoteactionaudits"></a><span data-ttu-id="d2f2b-103">Список Ремотеактионаудитс</span><span class="sxs-lookup"><span data-stu-id="d2f2b-103">List remoteActionAudits</span></span>

<span data-ttu-id="d2f2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2f2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2f2b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2f2b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2f2b-107">Список свойств и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="d2f2b-107">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2f2b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2f2b-108">Prerequisites</span></span>
<span data-ttu-id="d2f2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f2b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f2b-111">Permission type</span></span>|<span data-ttu-id="d2f2b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2f2b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f2b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f2b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d2f2b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2f2b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-116">Not supported.</span></span>|
|<span data-ttu-id="d2f2b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f2b-117">Application</span></span>|<span data-ttu-id="d2f2b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f2b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2f2b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="d2f2b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2f2b-120">Request headers</span></span>
|<span data-ttu-id="d2f2b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2f2b-121">Header</span></span>|<span data-ttu-id="d2f2b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2f2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2f2b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f2b-123">Authorization</span></span>|<span data-ttu-id="d2f2b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2f2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2f2b-125">Accept</span></span>|<span data-ttu-id="d2f2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2f2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f2b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f2b-127">Request body</span></span>
<span data-ttu-id="d2f2b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2f2b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2f2b-129">Response</span></span>
<span data-ttu-id="d2f2b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-130">If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f2b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f2b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2f2b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f2b-132">Request</span></span>
<span data-ttu-id="d2f2b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### <a name="response"></a><span data-ttu-id="d2f2b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f2b-134">Response</span></span>
<span data-ttu-id="d2f2b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2f2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



