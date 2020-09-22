---
title: Функция deviceConfigurationDeviceActivity
description: Метаданные для отчета о работе устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b814ff6a4143b7115d9c226243ca133bc632867d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971120"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="d8644-103">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="d8644-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="d8644-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8644-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8644-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8644-106">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="d8644-106">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8644-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d8644-107">Prerequisites</span></span>
<span data-ttu-id="d8644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8644-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8644-110">Permission type</span></span>|<span data-ttu-id="d8644-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8644-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8644-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8644-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8644-113">&nbsp;&nbsp;Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="d8644-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="d8644-114">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8644-114">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d8644-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8644-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8644-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8644-116">Not supported.</span></span>|
|<span data-ttu-id="d8644-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8644-117">Application</span></span>|<span data-ttu-id="d8644-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8644-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8644-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8644-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="d8644-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8644-120">Request headers</span></span>
|<span data-ttu-id="d8644-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8644-121">Header</span></span>|<span data-ttu-id="d8644-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8644-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8644-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8644-123">Authorization</span></span>|<span data-ttu-id="d8644-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8644-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8644-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8644-125">Accept</span></span>|<span data-ttu-id="d8644-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8644-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8644-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8644-127">Request body</span></span>
<span data-ttu-id="d8644-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8644-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8644-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8644-129">Response</span></span>
<span data-ttu-id="d8644-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8644-130">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8644-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8644-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8644-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8644-132">Request</span></span>
<span data-ttu-id="d8644-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8644-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="d8644-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8644-134">Response</span></span>
<span data-ttu-id="d8644-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8644-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```














