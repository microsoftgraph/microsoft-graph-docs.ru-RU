---
title: Получение Виндовсманажементапфеалссуммари
description: Чтение свойств и связей объекта Виндовсманажементапфеалссуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b45f8957fc744ea85719d1f1229c49eb9222a9ba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959168"
---
# <a name="get-windowsmanagementapphealthsummary"></a><span data-ttu-id="d60fd-103">Получение Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="d60fd-103">Get windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="d60fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d60fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d60fd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d60fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d60fd-106">Чтение свойств и связей объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d60fd-106">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d60fd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d60fd-107">Prerequisites</span></span>
<span data-ttu-id="d60fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d60fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d60fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d60fd-110">Permission type</span></span>|<span data-ttu-id="d60fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d60fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d60fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d60fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d60fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d60fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d60fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d60fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d60fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d60fd-115">Not supported.</span></span>|
|<span data-ttu-id="d60fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d60fd-116">Application</span></span>|<span data-ttu-id="d60fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d60fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d60fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d60fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d60fd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d60fd-119">Optional query parameters</span></span>
<span data-ttu-id="d60fd-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d60fd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d60fd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d60fd-121">Request headers</span></span>
|<span data-ttu-id="d60fd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d60fd-122">Header</span></span>|<span data-ttu-id="d60fd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d60fd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d60fd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d60fd-124">Authorization</span></span>|<span data-ttu-id="d60fd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d60fd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d60fd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d60fd-126">Accept</span></span>|<span data-ttu-id="d60fd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d60fd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d60fd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d60fd-128">Request body</span></span>
<span data-ttu-id="d60fd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d60fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d60fd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d60fd-130">Response</span></span>
<span data-ttu-id="d60fd-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d60fd-131">If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d60fd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d60fd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d60fd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d60fd-133">Request</span></span>
<span data-ttu-id="d60fd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d60fd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
```

### <a name="response"></a><span data-ttu-id="d60fd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d60fd-135">Response</span></span>
<span data-ttu-id="d60fd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d60fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
    "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
    "healthyDeviceCount": 2,
    "unhealthyDeviceCount": 4,
    "unknownDeviceCount": 2
  }
}
```




