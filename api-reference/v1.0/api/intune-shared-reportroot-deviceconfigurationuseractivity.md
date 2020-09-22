---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ed6adadb0c40e51db1b4e83489555f85156ef4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087266"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="7c2ea-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="7c2ea-103">deviceConfigurationUserActivity function</span></span>

<span data-ttu-id="7c2ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c2ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c2ea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c2ea-106">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="7c2ea-106">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c2ea-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c2ea-107">Prerequisites</span></span>
<span data-ttu-id="7c2ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c2ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c2ea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c2ea-110">Permission type</span></span>|<span data-ttu-id="7c2ea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c2ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c2ea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c2ea-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7c2ea-113">&nbsp;&nbsp;Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="7c2ea-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="7c2ea-114">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c2ea-114">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c2ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c2ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c2ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-116">Not supported.</span></span>|
|<span data-ttu-id="7c2ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c2ea-117">Application</span></span>|<span data-ttu-id="7c2ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c2ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c2ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="7c2ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c2ea-120">Request headers</span></span>
|<span data-ttu-id="7c2ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c2ea-121">Header</span></span>|<span data-ttu-id="7c2ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c2ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c2ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c2ea-123">Authorization</span></span>|<span data-ttu-id="7c2ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c2ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c2ea-125">Accept</span></span>|<span data-ttu-id="7c2ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c2ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c2ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c2ea-127">Request body</span></span>
<span data-ttu-id="7c2ea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c2ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c2ea-129">Response</span></span>
<span data-ttu-id="7c2ea-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-130">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c2ea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7c2ea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c2ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c2ea-132">Request</span></span>
<span data-ttu-id="7c2ea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="7c2ea-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c2ea-134">Response</span></span>
<span data-ttu-id="7c2ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c2ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














