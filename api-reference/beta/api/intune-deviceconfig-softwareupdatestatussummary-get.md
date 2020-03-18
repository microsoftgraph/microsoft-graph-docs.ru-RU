---
title: Получение объекта softwareUpdateStatusSummary
description: Чтение свойств и связей объекта softwareUpdateStatusSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3b304e8012c2b27d44ca0be24e48c1c5288cdb9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42741793"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="c500e-103">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="c500e-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="c500e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c500e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c500e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c500e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c500e-106">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c500e-106">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c500e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c500e-107">Prerequisites</span></span>
<span data-ttu-id="c500e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c500e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c500e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c500e-110">Permission type</span></span>|<span data-ttu-id="c500e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c500e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c500e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c500e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c500e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c500e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c500e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c500e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c500e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c500e-115">Not supported.</span></span>|
|<span data-ttu-id="c500e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c500e-116">Application</span></span>|<span data-ttu-id="c500e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c500e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c500e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c500e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c500e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c500e-119">Optional query parameters</span></span>
<span data-ttu-id="c500e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c500e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c500e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c500e-121">Request headers</span></span>
|<span data-ttu-id="c500e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c500e-122">Header</span></span>|<span data-ttu-id="c500e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c500e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c500e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c500e-124">Authorization</span></span>|<span data-ttu-id="c500e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c500e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c500e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c500e-126">Accept</span></span>|<span data-ttu-id="c500e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c500e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c500e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c500e-128">Request body</span></span>
<span data-ttu-id="c500e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c500e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c500e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c500e-130">Response</span></span>
<span data-ttu-id="c500e-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c500e-131">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c500e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c500e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c500e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c500e-133">Request</span></span>
<span data-ttu-id="c500e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c500e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="c500e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c500e-135">Response</span></span>
<span data-ttu-id="c500e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c500e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




