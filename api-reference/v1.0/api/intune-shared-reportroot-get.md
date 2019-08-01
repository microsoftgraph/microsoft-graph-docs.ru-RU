---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b767ae43a4b38a86665ad2f9d67c89acca33f81
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023414"
---
# <a name="get-reportroot"></a><span data-ttu-id="a1b89-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="a1b89-103">Get reportRoot</span></span>

> <span data-ttu-id="a1b89-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1b89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1b89-105">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="a1b89-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1b89-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a1b89-106">Prerequisites</span></span>
<span data-ttu-id="a1b89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1b89-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1b89-109">Permission type</span></span>|<span data-ttu-id="a1b89-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1b89-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1b89-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1b89-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a1b89-112">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="a1b89-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="a1b89-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1b89-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a1b89-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="a1b89-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="a1b89-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1b89-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a1b89-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1b89-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1b89-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1b89-117">Not supported.</span></span>|
|<span data-ttu-id="a1b89-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1b89-118">Application</span></span>|<span data-ttu-id="a1b89-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1b89-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1b89-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1b89-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1b89-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1b89-121">Optional query parameters</span></span>
<span data-ttu-id="a1b89-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1b89-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a1b89-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1b89-123">Request headers</span></span>
|<span data-ttu-id="a1b89-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1b89-124">Header</span></span>|<span data-ttu-id="a1b89-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a1b89-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1b89-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1b89-126">Authorization</span></span>|<span data-ttu-id="a1b89-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1b89-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1b89-128">Accept</span><span class="sxs-lookup"><span data-stu-id="a1b89-128">Accept</span></span>|<span data-ttu-id="a1b89-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a1b89-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1b89-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1b89-130">Request body</span></span>
<span data-ttu-id="a1b89-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1b89-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1b89-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1b89-132">Response</span></span>
<span data-ttu-id="a1b89-133">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a1b89-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1b89-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a1b89-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1b89-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1b89-135">Request</span></span>
<span data-ttu-id="a1b89-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1b89-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="a1b89-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1b89-137">Response</span></span>
<span data-ttu-id="a1b89-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1b89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








