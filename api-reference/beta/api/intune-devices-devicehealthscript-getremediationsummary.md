---
title: Функция Жетремедиатионсуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1fab0910bab555bfc696c6fe2faa1081c61b8fb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203419"
---
# <a name="getremediationsummary-function"></a><span data-ttu-id="e8f17-103">Функция Жетремедиатионсуммари</span><span class="sxs-lookup"><span data-stu-id="e8f17-103">getRemediationSummary function</span></span>

<span data-ttu-id="e8f17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8f17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8f17-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8f17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f17-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8f17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f17-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e8f17-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8f17-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8f17-108">Prerequisites</span></span>
<span data-ttu-id="e8f17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8f17-111">Permission type</span></span>|<span data-ttu-id="e8f17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8f17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8f17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8f17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e8f17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8f17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8f17-116">Not supported.</span></span>|
|<span data-ttu-id="e8f17-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8f17-117">Application</span></span>|<span data-ttu-id="e8f17-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8f17-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8f17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/getRemediationSummary
```

## <a name="request-headers"></a><span data-ttu-id="e8f17-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8f17-120">Request headers</span></span>
|<span data-ttu-id="e8f17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8f17-121">Header</span></span>|<span data-ttu-id="e8f17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8f17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8f17-123">Authorization</span></span>|<span data-ttu-id="e8f17-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8f17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8f17-125">Accept</span></span>|<span data-ttu-id="e8f17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8f17-127">Request body</span></span>
<span data-ttu-id="e8f17-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8f17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8f17-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8f17-129">Response</span></span>
<span data-ttu-id="e8f17-130">В случае успеха эта функция возвращает `200 OK` код отклика и объект [девицехеалсскриптремедиатионсуммари](../resources/intune-devices-devicehealthscriptremediationsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8f17-130">If successful, this function returns a `200 OK` response code and a [deviceHealthScriptRemediationSummary](../resources/intune-devices-devicehealthscriptremediationsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8f17-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e8f17-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8f17-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8f17-132">Request</span></span>
<span data-ttu-id="e8f17-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8f17-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/getRemediationSummary
```

### <a name="response"></a><span data-ttu-id="e8f17-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8f17-134">Response</span></span>
<span data-ttu-id="e8f17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8f17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "value": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary",
    "scriptCount": 11,
    "remediatedDeviceCount": 5
  }
}
```




