---
title: Действие refreshDeviceComplianceReportSummarization
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5428ac49c9ee9409aaedd0e3097c824000f43ead
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201080"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="5f9e1-103">Действие refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="5f9e1-103">refreshDeviceComplianceReportSummarization action</span></span>

> <span data-ttu-id="5f9e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f9e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f9e1-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f9e1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5f9e1-107">Prerequisites</span></span>
<span data-ttu-id="5f9e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f9e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f9e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f9e1-110">Permission type</span></span>|<span data-ttu-id="5f9e1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f9e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f9e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f9e1-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5f9e1-113">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="5f9e1-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5f9e1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f9e1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f9e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f9e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f9e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-116">Not supported.</span></span>|
|<span data-ttu-id="5f9e1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f9e1-117">Application</span></span>||
| <span data-ttu-id="5f9e1-118">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="5f9e1-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5f9e1-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f9e1-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f9e1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f9e1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="5f9e1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f9e1-121">Request headers</span></span>
|<span data-ttu-id="5f9e1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f9e1-122">Header</span></span>|<span data-ttu-id="5f9e1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5f9e1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f9e1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f9e1-124">Authorization</span></span>|<span data-ttu-id="5f9e1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f9e1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5f9e1-126">Accept</span></span>|<span data-ttu-id="5f9e1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5f9e1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f9e1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5f9e1-128">Request body</span></span>
<span data-ttu-id="5f9e1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f9e1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f9e1-130">Response</span></span>
<span data-ttu-id="5f9e1-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f9e1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5f9e1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f9e1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f9e1-133">Request</span></span>
<span data-ttu-id="5f9e1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="5f9e1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f9e1-135">Response</span></span>
<span data-ttu-id="5f9e1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f9e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




