---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61e346a1759c643965e24bff62da62974b1adc2c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760772"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="f0d5a-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="f0d5a-103">deviceConfigurationUserActivity function</span></span>

<span data-ttu-id="f0d5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0d5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0d5a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0d5a-106">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="f0d5a-106">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0d5a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0d5a-107">Prerequisites</span></span>
<span data-ttu-id="f0d5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0d5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0d5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0d5a-110">Permission type</span></span>|<span data-ttu-id="f0d5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0d5a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0d5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0d5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0d5a-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0d5a-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f0d5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0d5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0d5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-115">Not supported.</span></span>|
|<span data-ttu-id="f0d5a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0d5a-116">Application</span></span>|<span data-ttu-id="f0d5a-117">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0d5a-117">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0d5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0d5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="f0d5a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0d5a-119">Request headers</span></span>
|<span data-ttu-id="f0d5a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0d5a-120">Header</span></span>|<span data-ttu-id="f0d5a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f0d5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0d5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d5a-122">Authorization</span></span>|<span data-ttu-id="f0d5a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0d5a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f0d5a-124">Accept</span></span>|<span data-ttu-id="f0d5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0d5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0d5a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0d5a-126">Request body</span></span>
<span data-ttu-id="f0d5a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0d5a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0d5a-128">Response</span></span>
<span data-ttu-id="f0d5a-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-deviceconfig-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-deviceconfig-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0d5a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f0d5a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0d5a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0d5a-131">Request</span></span>
<span data-ttu-id="f0d5a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="f0d5a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0d5a-133">Response</span></span>
<span data-ttu-id="f0d5a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0d5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




