---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9c1e248ef9e6a8803f63c78656e57977ee20f43
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865427"
---
# <a name="get-reportroot"></a><span data-ttu-id="ee68d-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="ee68d-103">Get reportRoot</span></span>

<span data-ttu-id="ee68d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee68d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee68d-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="ee68d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee68d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee68d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee68d-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee68d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee68d-108">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ee68d-108">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee68d-109">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ee68d-109">Prerequisites</span></span>
<span data-ttu-id="ee68d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee68d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee68d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee68d-112">Permission type</span></span>|<span data-ttu-id="ee68d-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee68d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee68d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee68d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ee68d-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="ee68d-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ee68d-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee68d-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ee68d-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="ee68d-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ee68d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee68d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ee68d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee68d-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee68d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee68d-120">Not supported.</span></span>|
|<span data-ttu-id="ee68d-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ee68d-121">Application</span></span>||
| <span data-ttu-id="ee68d-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="ee68d-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ee68d-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee68d-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ee68d-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="ee68d-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ee68d-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee68d-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee68d-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee68d-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee68d-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee68d-127">Optional query parameters</span></span>
<span data-ttu-id="ee68d-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee68d-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ee68d-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee68d-129">Request headers</span></span>
|<span data-ttu-id="ee68d-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee68d-130">Header</span></span>|<span data-ttu-id="ee68d-131">Значение</span><span class="sxs-lookup"><span data-stu-id="ee68d-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee68d-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee68d-132">Authorization</span></span>|<span data-ttu-id="ee68d-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee68d-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee68d-134">Accept</span><span class="sxs-lookup"><span data-stu-id="ee68d-134">Accept</span></span>|<span data-ttu-id="ee68d-135">application/json</span><span class="sxs-lookup"><span data-stu-id="ee68d-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee68d-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee68d-136">Request body</span></span>
<span data-ttu-id="ee68d-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee68d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee68d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee68d-138">Response</span></span>
<span data-ttu-id="ee68d-139">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee68d-139">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee68d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ee68d-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee68d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee68d-141">Request</span></span>
<span data-ttu-id="ee68d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee68d-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="ee68d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee68d-143">Response</span></span>
<span data-ttu-id="ee68d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee68d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










