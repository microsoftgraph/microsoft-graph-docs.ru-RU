---
title: Get managedAppStatus
description: Чтение свойств и связей объекта managedAppStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f800975c9d209ef6ad818348a8dfe61b78e8bd3c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954393"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="88e6e-103">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="88e6e-103">Get managedAppStatus</span></span>

> <span data-ttu-id="88e6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88e6e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88e6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88e6e-106">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="88e6e-106">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88e6e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="88e6e-107">Prerequisites</span></span>
<span data-ttu-id="88e6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88e6e-110">Permission type</span></span>|<span data-ttu-id="88e6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88e6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88e6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88e6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88e6e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e6e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="88e6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88e6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88e6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e6e-115">Not supported.</span></span>|
|<span data-ttu-id="88e6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88e6e-116">Application</span></span>|<span data-ttu-id="88e6e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e6e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88e6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88e6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88e6e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88e6e-119">Optional query parameters</span></span>
<span data-ttu-id="88e6e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="88e6e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88e6e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88e6e-121">Request headers</span></span>
|<span data-ttu-id="88e6e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88e6e-122">Header</span></span>|<span data-ttu-id="88e6e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="88e6e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88e6e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88e6e-124">Authorization</span></span>|<span data-ttu-id="88e6e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88e6e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88e6e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="88e6e-126">Accept</span></span>|<span data-ttu-id="88e6e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="88e6e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88e6e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88e6e-128">Request body</span></span>
<span data-ttu-id="88e6e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88e6e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88e6e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="88e6e-130">Response</span></span>
<span data-ttu-id="88e6e-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatus](../resources/intune-mam-managedappstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="88e6e-131">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e6e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="88e6e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="88e6e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="88e6e-133">Request</span></span>
<span data-ttu-id="88e6e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88e6e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="88e6e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="88e6e-135">Response</span></span>
<span data-ttu-id="88e6e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88e6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatus",
    "displayName": "Display Name value",
    "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
    "version": "Version value"
  }
}
```





