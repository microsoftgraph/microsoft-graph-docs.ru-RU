---
title: Получение объекта softwareUpdateStatusSummary
description: Чтение свойств и связей объекта softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9bac9fd4f19cf1812a8a21ffff78d91db750aca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020298"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="c85bc-103">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="c85bc-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="c85bc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c85bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c85bc-105">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c85bc-105">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c85bc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c85bc-106">Prerequisites</span></span>
<span data-ttu-id="c85bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c85bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c85bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c85bc-109">Permission type</span></span>|<span data-ttu-id="c85bc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c85bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c85bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c85bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c85bc-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c85bc-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c85bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c85bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c85bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c85bc-114">Not supported.</span></span>|
|<span data-ttu-id="c85bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c85bc-115">Application</span></span>|<span data-ttu-id="c85bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c85bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c85bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c85bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c85bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c85bc-118">Optional query parameters</span></span>
<span data-ttu-id="c85bc-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c85bc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c85bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c85bc-120">Request headers</span></span>
|<span data-ttu-id="c85bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c85bc-121">Header</span></span>|<span data-ttu-id="c85bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c85bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c85bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c85bc-123">Authorization</span></span>|<span data-ttu-id="c85bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c85bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c85bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c85bc-125">Accept</span></span>|<span data-ttu-id="c85bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c85bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c85bc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c85bc-127">Request body</span></span>
<span data-ttu-id="c85bc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c85bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c85bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c85bc-129">Response</span></span>
<span data-ttu-id="c85bc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c85bc-130">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c85bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c85bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c85bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c85bc-132">Request</span></span>
<span data-ttu-id="c85bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c85bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="c85bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c85bc-134">Response</span></span>
<span data-ttu-id="c85bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c85bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



