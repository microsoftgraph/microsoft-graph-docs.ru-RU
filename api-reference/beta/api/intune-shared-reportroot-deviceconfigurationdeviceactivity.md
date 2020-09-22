---
title: Функция deviceConfigurationDeviceActivity
description: Метаданные для отчета о работе устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7fef29e115bd206d90327ec40e1e5b79be109aaa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068058"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="18aa9-103">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="18aa9-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="18aa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18aa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18aa9-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18aa9-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18aa9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18aa9-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18aa9-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18aa9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18aa9-108">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="18aa9-108">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18aa9-109">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="18aa9-109">Prerequisites</span></span>
<span data-ttu-id="18aa9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18aa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18aa9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18aa9-112">Permission type</span></span>|<span data-ttu-id="18aa9-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18aa9-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18aa9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18aa9-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="18aa9-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="18aa9-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="18aa9-116">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18aa9-116">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18aa9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18aa9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18aa9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18aa9-118">Not supported.</span></span>|
|<span data-ttu-id="18aa9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18aa9-119">Application</span></span>||
| <span data-ttu-id="18aa9-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="18aa9-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="18aa9-121">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18aa9-121">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18aa9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18aa9-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="18aa9-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18aa9-123">Request headers</span></span>
|<span data-ttu-id="18aa9-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18aa9-124">Header</span></span>|<span data-ttu-id="18aa9-125">Значение</span><span class="sxs-lookup"><span data-stu-id="18aa9-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18aa9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18aa9-126">Authorization</span></span>|<span data-ttu-id="18aa9-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18aa9-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18aa9-128">Accept</span><span class="sxs-lookup"><span data-stu-id="18aa9-128">Accept</span></span>|<span data-ttu-id="18aa9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="18aa9-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18aa9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18aa9-130">Request body</span></span>
<span data-ttu-id="18aa9-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18aa9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18aa9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="18aa9-132">Response</span></span>
<span data-ttu-id="18aa9-133">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18aa9-133">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18aa9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="18aa9-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="18aa9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="18aa9-135">Request</span></span>
<span data-ttu-id="18aa9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18aa9-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="18aa9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="18aa9-137">Response</span></span>
<span data-ttu-id="18aa9-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18aa9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












