---
title: Действие refreshDeviceComplianceReportSummarization
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3671b01dced9b738bcfab5f57331a1a1a8789bc
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536184"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="f7c6f-103">Действие refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="f7c6f-103">refreshDeviceComplianceReportSummarization action</span></span>

> <span data-ttu-id="f7c6f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7c6f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7c6f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7c6f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7c6f-107">Prerequisites</span></span>
<span data-ttu-id="f7c6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c6f-110">Permission type</span></span>|<span data-ttu-id="f7c6f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7c6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c6f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f7c6f-113">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f7c6f-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f7c6f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7c6f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f7c6f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-116">Not supported.</span></span>|
|<span data-ttu-id="f7c6f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f7c6f-117">Application</span></span>||
| <span data-ttu-id="f7c6f-118">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="f7c6f-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f7c6f-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7c6f-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7c6f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c6f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="f7c6f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7c6f-121">Request headers</span></span>
|<span data-ttu-id="f7c6f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7c6f-122">Header</span></span>|<span data-ttu-id="f7c6f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f7c6f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7c6f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7c6f-124">Authorization</span></span>|<span data-ttu-id="f7c6f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7c6f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f7c6f-126">Accept</span></span>|<span data-ttu-id="f7c6f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c6f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c6f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7c6f-128">Request body</span></span>
<span data-ttu-id="f7c6f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7c6f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7c6f-130">Response</span></span>
<span data-ttu-id="f7c6f-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7c6f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c6f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7c6f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c6f-133">Request</span></span>
<span data-ttu-id="f7c6f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="f7c6f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c6f-135">Response</span></span>
<span data-ttu-id="f7c6f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7c6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






