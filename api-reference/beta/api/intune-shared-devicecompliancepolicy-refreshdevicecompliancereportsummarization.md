---
title: Действие refreshDeviceComplianceReportSummarization
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8de8d91ebbc13ffe83bf3873fe3874bf7cfad81e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390753"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="bca13-103">Действие refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="bca13-103">refreshDeviceComplianceReportSummarization action</span></span>

<span data-ttu-id="bca13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bca13-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca13-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bca13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca13-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bca13-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bca13-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bca13-108">Prerequisites</span></span>
<span data-ttu-id="bca13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bca13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bca13-111">Permission type</span></span>|<span data-ttu-id="bca13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bca13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bca13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bca13-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bca13-114">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="bca13-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bca13-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bca13-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bca13-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bca13-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bca13-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca13-117">Not supported.</span></span>|
|<span data-ttu-id="bca13-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bca13-118">Application</span></span>||
| <span data-ttu-id="bca13-119">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="bca13-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bca13-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bca13-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bca13-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bca13-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="bca13-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bca13-122">Request headers</span></span>
|<span data-ttu-id="bca13-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bca13-123">Header</span></span>|<span data-ttu-id="bca13-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bca13-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bca13-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bca13-125">Authorization</span></span>|<span data-ttu-id="bca13-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bca13-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bca13-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bca13-127">Accept</span></span>|<span data-ttu-id="bca13-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bca13-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca13-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bca13-129">Request body</span></span>
<span data-ttu-id="bca13-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bca13-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bca13-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bca13-131">Response</span></span>
<span data-ttu-id="bca13-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bca13-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bca13-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bca13-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bca13-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bca13-134">Request</span></span>
<span data-ttu-id="bca13-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bca13-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="bca13-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bca13-136">Response</span></span>
<span data-ttu-id="bca13-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bca13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






