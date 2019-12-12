---
title: Get managedAppStatusRaw
description: Чтение свойств и связей объекта managedAppStatusRaw.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56cb8c1aed297a7b0be719bea94b5518e9ed086d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954379"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="ece33-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="ece33-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="ece33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ece33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ece33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece33-106">Чтение свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="ece33-106">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ece33-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ece33-107">Prerequisites</span></span>
<span data-ttu-id="ece33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ece33-110">Permission type</span></span>|<span data-ttu-id="ece33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ece33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ece33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ece33-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ece33-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ece33-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ece33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece33-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece33-115">Not supported.</span></span>|
|<span data-ttu-id="ece33-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ece33-116">Application</span></span>|<span data-ttu-id="ece33-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ece33-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece33-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ece33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ece33-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ece33-119">Optional query parameters</span></span>
<span data-ttu-id="ece33-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ece33-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ece33-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ece33-121">Request headers</span></span>
|<span data-ttu-id="ece33-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ece33-122">Header</span></span>|<span data-ttu-id="ece33-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ece33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece33-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ece33-124">Authorization</span></span>|<span data-ttu-id="ece33-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ece33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece33-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ece33-126">Accept</span></span>|<span data-ttu-id="ece33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ece33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece33-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ece33-128">Request body</span></span>
<span data-ttu-id="ece33-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ece33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ece33-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ece33-130">Response</span></span>
<span data-ttu-id="ece33-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ece33-131">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece33-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ece33-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ece33-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ece33-133">Request</span></span>
<span data-ttu-id="ece33-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ece33-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="ece33-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ece33-135">Response</span></span>
<span data-ttu-id="ece33-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ece33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```





