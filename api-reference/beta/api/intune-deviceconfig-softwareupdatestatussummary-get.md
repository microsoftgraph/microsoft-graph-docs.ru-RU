---
title: Получение объекта softwareUpdateStatusSummary
description: Чтение свойств и связей объекта softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3a769608a924205f5bf458cbfc6b7a258bd1339
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734982"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="bd8bc-103">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="bd8bc-103">Get softwareUpdateStatusSummary</span></span>

<span data-ttu-id="bd8bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd8bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd8bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd8bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd8bc-107">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="bd8bc-107">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd8bc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bd8bc-108">Prerequisites</span></span>
<span data-ttu-id="bd8bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd8bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd8bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd8bc-111">Permission type</span></span>|<span data-ttu-id="bd8bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd8bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd8bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd8bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd8bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd8bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bd8bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd8bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd8bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-116">Not supported.</span></span>|
|<span data-ttu-id="bd8bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd8bc-117">Application</span></span>|<span data-ttu-id="bd8bc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd8bc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd8bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd8bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd8bc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd8bc-120">Optional query parameters</span></span>
<span data-ttu-id="bd8bc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd8bc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd8bc-122">Request headers</span></span>
|<span data-ttu-id="bd8bc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd8bc-123">Header</span></span>|<span data-ttu-id="bd8bc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bd8bc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd8bc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd8bc-125">Authorization</span></span>|<span data-ttu-id="bd8bc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd8bc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bd8bc-127">Accept</span></span>|<span data-ttu-id="bd8bc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bd8bc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd8bc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd8bc-129">Request body</span></span>
<span data-ttu-id="bd8bc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd8bc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd8bc-131">Response</span></span>
<span data-ttu-id="bd8bc-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-132">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd8bc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bd8bc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd8bc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd8bc-134">Request</span></span>
<span data-ttu-id="bd8bc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="bd8bc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd8bc-136">Response</span></span>
<span data-ttu-id="bd8bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd8bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```





