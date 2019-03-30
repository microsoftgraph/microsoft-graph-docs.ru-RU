---
title: Действие refreshDeviceComplianceReportSummarization
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68a52635930a8bcb77d33b26c68ce53a855d51c4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985986"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="fdd39-103">Действие refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="fdd39-103">refreshDeviceComplianceReportSummarization action</span></span>

> <span data-ttu-id="fdd39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdd39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdd39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdd39-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fdd39-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdd39-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fdd39-107">Prerequisites</span></span>
<span data-ttu-id="fdd39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdd39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdd39-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd39-110">Permission type</span></span>|<span data-ttu-id="fdd39-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdd39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdd39-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdd39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdd39-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdd39-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fdd39-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdd39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdd39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd39-115">Not supported.</span></span>|
|<span data-ttu-id="fdd39-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdd39-116">Application</span></span>|<span data-ttu-id="fdd39-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdd39-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdd39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="fdd39-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdd39-119">Request headers</span></span>
|<span data-ttu-id="fdd39-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdd39-120">Header</span></span>|<span data-ttu-id="fdd39-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fdd39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdd39-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdd39-122">Authorization</span></span>|<span data-ttu-id="fdd39-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdd39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdd39-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fdd39-124">Accept</span></span>|<span data-ttu-id="fdd39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fdd39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdd39-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdd39-126">Request body</span></span>
<span data-ttu-id="fdd39-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdd39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdd39-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdd39-128">Response</span></span>
<span data-ttu-id="fdd39-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fdd39-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fdd39-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fdd39-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdd39-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdd39-131">Request</span></span>
<span data-ttu-id="fdd39-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdd39-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="fdd39-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdd39-133">Response</span></span>
<span data-ttu-id="fdd39-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdd39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




