---
title: Перечисление объектов managedAppStatusRaw
description: Список свойств и связей объектов managedAppStatusRaw.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ed40045e1f9e823bba88b9b551470de0ed1fc13
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803479"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="e147e-103">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="e147e-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="e147e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e147e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e147e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e147e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e147e-106">Список свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="e147e-106">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e147e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e147e-107">Prerequisites</span></span>
<span data-ttu-id="e147e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e147e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e147e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e147e-110">Permission type</span></span>|<span data-ttu-id="e147e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e147e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e147e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e147e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e147e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e147e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e147e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e147e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e147e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e147e-115">Not supported.</span></span>|
|<span data-ttu-id="e147e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e147e-116">Application</span></span>|<span data-ttu-id="e147e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e147e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e147e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e147e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e147e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e147e-119">Request headers</span></span>
|<span data-ttu-id="e147e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e147e-120">Header</span></span>|<span data-ttu-id="e147e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e147e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e147e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e147e-122">Authorization</span></span>|<span data-ttu-id="e147e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e147e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e147e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e147e-124">Accept</span></span>|<span data-ttu-id="e147e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e147e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e147e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e147e-126">Request body</span></span>
<span data-ttu-id="e147e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e147e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e147e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e147e-128">Response</span></span>
<span data-ttu-id="e147e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e147e-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e147e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e147e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e147e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e147e-131">Request</span></span>
<span data-ttu-id="e147e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e147e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="e147e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e147e-133">Response</span></span>
<span data-ttu-id="e147e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e147e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```




