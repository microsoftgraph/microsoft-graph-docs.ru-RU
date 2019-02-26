---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e24a86c1ff4443b0d2867dc9f7da7e273a3012e0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251911"
---
# <a name="get-reportroot"></a><span data-ttu-id="13b99-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="13b99-103">Get reportRoot</span></span>

> <span data-ttu-id="13b99-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13b99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13b99-105">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="13b99-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13b99-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="13b99-106">Prerequisites</span></span>
<span data-ttu-id="13b99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13b99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13b99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13b99-109">Permission type</span></span>|<span data-ttu-id="13b99-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13b99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13b99-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13b99-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="13b99-112">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="13b99-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="13b99-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13b99-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="13b99-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="13b99-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="13b99-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="13b99-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="13b99-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13b99-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13b99-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13b99-117">Not supported.</span></span>|
|<span data-ttu-id="13b99-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13b99-118">Application</span></span>|<span data-ttu-id="13b99-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13b99-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13b99-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13b99-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13b99-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13b99-121">Optional query parameters</span></span>
<span data-ttu-id="13b99-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="13b99-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="13b99-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13b99-123">Request headers</span></span>
|<span data-ttu-id="13b99-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13b99-124">Header</span></span>|<span data-ttu-id="13b99-125">Значение</span><span class="sxs-lookup"><span data-stu-id="13b99-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13b99-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="13b99-126">Authorization</span></span>|<span data-ttu-id="13b99-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="13b99-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13b99-128">Accept</span><span class="sxs-lookup"><span data-stu-id="13b99-128">Accept</span></span>|<span data-ttu-id="13b99-129">application/json</span><span class="sxs-lookup"><span data-stu-id="13b99-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13b99-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13b99-130">Request body</span></span>
<span data-ttu-id="13b99-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13b99-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13b99-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="13b99-132">Response</span></span>
<span data-ttu-id="13b99-133">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="13b99-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13b99-134">Пример</span><span class="sxs-lookup"><span data-stu-id="13b99-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="13b99-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="13b99-135">Request</span></span>
<span data-ttu-id="13b99-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13b99-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="13b99-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="13b99-137">Response</span></span>
<span data-ttu-id="13b99-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="13b99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








