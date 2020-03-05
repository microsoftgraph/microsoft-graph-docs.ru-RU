---
title: Действие refreshDeviceComplianceReportSummarization
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aef20301d5a781f0e76421779d65711232fb90da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458688"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="0d32c-103">Действие refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="0d32c-103">refreshDeviceComplianceReportSummarization action</span></span>

<span data-ttu-id="0d32c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0d32c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d32c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d32c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d32c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d32c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d32c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0d32c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d32c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d32c-108">Prerequisites</span></span>
<span data-ttu-id="0d32c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d32c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d32c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d32c-111">Permission type</span></span>|<span data-ttu-id="0d32c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d32c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d32c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d32c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0d32c-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="0d32c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0d32c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d32c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0d32c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d32c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d32c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d32c-117">Not supported.</span></span>|
|<span data-ttu-id="0d32c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d32c-118">Application</span></span>||
| <span data-ttu-id="0d32c-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="0d32c-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0d32c-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d32c-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d32c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d32c-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="0d32c-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d32c-122">Request headers</span></span>
|<span data-ttu-id="0d32c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d32c-123">Header</span></span>|<span data-ttu-id="0d32c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0d32c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d32c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d32c-125">Authorization</span></span>|<span data-ttu-id="0d32c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d32c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d32c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0d32c-127">Accept</span></span>|<span data-ttu-id="0d32c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d32c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d32c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d32c-129">Request body</span></span>
<span data-ttu-id="0d32c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d32c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d32c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d32c-131">Response</span></span>
<span data-ttu-id="0d32c-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d32c-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d32c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0d32c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d32c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d32c-134">Request</span></span>
<span data-ttu-id="0d32c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d32c-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="0d32c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d32c-136">Response</span></span>
<span data-ttu-id="0d32c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d32c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








