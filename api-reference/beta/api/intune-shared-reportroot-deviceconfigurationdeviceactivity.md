---
title: Функция deviceConfigurationDeviceActivity
description: Метаданные для отчета о работе устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ff6856cd31564664847e65a26b66a160d9cf4ff
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694223"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="dfffd-103">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="dfffd-103">deviceConfigurationDeviceActivity function</span></span>

<span data-ttu-id="dfffd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfffd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfffd-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dfffd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dfffd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfffd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfffd-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfffd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfffd-108">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="dfffd-108">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dfffd-109">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dfffd-109">Prerequisites</span></span>
<span data-ttu-id="dfffd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfffd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfffd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfffd-112">Permission type</span></span>|<span data-ttu-id="dfffd-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfffd-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfffd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfffd-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dfffd-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="dfffd-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="dfffd-116">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfffd-116">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dfffd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfffd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfffd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfffd-118">Not supported.</span></span>|
|<span data-ttu-id="dfffd-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfffd-119">Application</span></span>||
| <span data-ttu-id="dfffd-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="dfffd-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="dfffd-121">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfffd-121">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfffd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfffd-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="dfffd-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dfffd-123">Request headers</span></span>
|<span data-ttu-id="dfffd-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfffd-124">Header</span></span>|<span data-ttu-id="dfffd-125">Значение</span><span class="sxs-lookup"><span data-stu-id="dfffd-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfffd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfffd-126">Authorization</span></span>|<span data-ttu-id="dfffd-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfffd-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfffd-128">Accept</span><span class="sxs-lookup"><span data-stu-id="dfffd-128">Accept</span></span>|<span data-ttu-id="dfffd-129">application/json</span><span class="sxs-lookup"><span data-stu-id="dfffd-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfffd-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfffd-130">Request body</span></span>
<span data-ttu-id="dfffd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfffd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfffd-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfffd-132">Response</span></span>
<span data-ttu-id="dfffd-133">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfffd-133">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfffd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dfffd-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="dfffd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfffd-135">Request</span></span>
<span data-ttu-id="dfffd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfffd-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="dfffd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfffd-137">Response</span></span>
<span data-ttu-id="dfffd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfffd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











