---
title: Получение объекта softwareUpdateStatusSummary
description: Чтение свойств и связей объекта softwareUpdateStatusSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 914ddc3be9b0e964a63a42163a498b686a3749ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946336"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="cd9bb-103">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cd9bb-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="cd9bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd9bb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd9bb-106">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="cd9bb-106">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd9bb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cd9bb-107">Prerequisites</span></span>
<span data-ttu-id="cd9bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd9bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd9bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9bb-110">Permission type</span></span>|<span data-ttu-id="cd9bb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd9bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd9bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd9bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cd9bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd9bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9bb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-115">Not supported.</span></span>|
|<span data-ttu-id="cd9bb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd9bb-116">Application</span></span>|<span data-ttu-id="cd9bb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9bb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd9bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd9bb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cd9bb-119">Optional query parameters</span></span>
<span data-ttu-id="cd9bb-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd9bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd9bb-121">Request headers</span></span>
|<span data-ttu-id="cd9bb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd9bb-122">Header</span></span>|<span data-ttu-id="cd9bb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cd9bb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd9bb-124">Authorization</span></span>|<span data-ttu-id="cd9bb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd9bb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cd9bb-126">Accept</span></span>|<span data-ttu-id="cd9bb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9bb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9bb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd9bb-128">Request body</span></span>
<span data-ttu-id="cd9bb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd9bb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd9bb-130">Response</span></span>
<span data-ttu-id="cd9bb-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-131">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9bb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cd9bb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd9bb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd9bb-133">Request</span></span>
<span data-ttu-id="cd9bb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="cd9bb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd9bb-135">Response</span></span>
<span data-ttu-id="cd9bb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd9bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





