---
title: Функция deviceConfigurationDeviceActivity
description: Метаданные для отчета о работе устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 036c21514e0833182e2957cf78cb2f98cbbf253e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760773"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="c54d9-103">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="c54d9-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="c54d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c54d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c54d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c54d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c54d9-106">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="c54d9-106">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c54d9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c54d9-107">Prerequisites</span></span>
<span data-ttu-id="c54d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c54d9-110">Permission type</span></span>|<span data-ttu-id="c54d9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c54d9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c54d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c54d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c54d9-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c54d9-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c54d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c54d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c54d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c54d9-115">Not supported.</span></span>|
|<span data-ttu-id="c54d9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c54d9-116">Application</span></span>|<span data-ttu-id="c54d9-117">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c54d9-117">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c54d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c54d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="c54d9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c54d9-119">Request headers</span></span>
|<span data-ttu-id="c54d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c54d9-120">Header</span></span>|<span data-ttu-id="c54d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c54d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c54d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c54d9-122">Authorization</span></span>|<span data-ttu-id="c54d9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c54d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c54d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c54d9-124">Accept</span></span>|<span data-ttu-id="c54d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c54d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c54d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c54d9-126">Request body</span></span>
<span data-ttu-id="c54d9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c54d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c54d9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c54d9-128">Response</span></span>
<span data-ttu-id="c54d9-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-deviceconfig-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c54d9-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-deviceconfig-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c54d9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c54d9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c54d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c54d9-131">Request</span></span>
<span data-ttu-id="c54d9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c54d9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="c54d9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c54d9-133">Response</span></span>
<span data-ttu-id="c54d9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c54d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "Y29udGVudCBJbnR1bmUgRG9jIFNhbXBsZSAxNTYxOTcwNjY1"
  }
}
```




