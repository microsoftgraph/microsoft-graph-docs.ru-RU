---
title: функция getRemediationHistory
description: Функция получения количества исправлений скриптами для здоровья устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 807bf35837a9c731c426f6376ef14913119b4911
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146309"
---
# <a name="getremediationhistory-function"></a><span data-ttu-id="f395b-103">функция getRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="f395b-103">getRemediationHistory function</span></span>

<span data-ttu-id="f395b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f395b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f395b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f395b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f395b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f395b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f395b-107">Функция получения количества исправлений скриптами для здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="f395b-107">Function to get the number of remediations by a device health scripts</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f395b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f395b-108">Prerequisites</span></span>
<span data-ttu-id="f395b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f395b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f395b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f395b-111">Permission type</span></span>|<span data-ttu-id="f395b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f395b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f395b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f395b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f395b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f395b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f395b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f395b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f395b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f395b-116">Not supported.</span></span>|
|<span data-ttu-id="f395b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f395b-117">Application</span></span>|<span data-ttu-id="f395b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f395b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f395b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f395b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

## <a name="request-headers"></a><span data-ttu-id="f395b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f395b-120">Request headers</span></span>
|<span data-ttu-id="f395b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f395b-121">Header</span></span>|<span data-ttu-id="f395b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f395b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f395b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f395b-123">Authorization</span></span>|<span data-ttu-id="f395b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f395b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f395b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f395b-125">Accept</span></span>|<span data-ttu-id="f395b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f395b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f395b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f395b-127">Request body</span></span>
<span data-ttu-id="f395b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f395b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f395b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f395b-129">Response</span></span>
<span data-ttu-id="f395b-130">В случае успешной данной функции возвращается код ответа и `200 OK` [устройствоHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f395b-130">If successful, this function returns a `200 OK` response code and a [deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f395b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f395b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f395b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f395b-132">Request</span></span>
<span data-ttu-id="f395b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f395b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

### <a name="response"></a><span data-ttu-id="f395b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f395b-134">Response</span></span>
<span data-ttu-id="f395b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f395b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "historyData": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
        "date": "2016-12-31",
        "remediatedDeviceCount": 5,
        "noIssueDeviceCount": 2
      }
    ]
  }
}
```




