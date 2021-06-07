---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b7c109af425119ac02f6ee9bbac944ebfa03629
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755521"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="58c5e-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="58c5e-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

<span data-ttu-id="58c5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58c5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58c5e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58c5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58c5e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58c5e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58c5e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58c5e-107">Prerequisites</span></span>
<span data-ttu-id="58c5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58c5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58c5e-110">Permission type</span></span>|<span data-ttu-id="58c5e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58c5e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58c5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58c5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58c5e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58c5e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58c5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58c5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58c5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58c5e-115">Not supported.</span></span>|
|<span data-ttu-id="58c5e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="58c5e-116">Application</span></span>|<span data-ttu-id="58c5e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58c5e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58c5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58c5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="58c5e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58c5e-119">Request headers</span></span>
|<span data-ttu-id="58c5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58c5e-120">Header</span></span>|<span data-ttu-id="58c5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58c5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58c5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58c5e-122">Authorization</span></span>|<span data-ttu-id="58c5e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58c5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58c5e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58c5e-124">Accept</span></span>|<span data-ttu-id="58c5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58c5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58c5e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58c5e-126">Request body</span></span>
<span data-ttu-id="58c5e-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="58c5e-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="58c5e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="58c5e-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="58c5e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58c5e-129">Property</span></span>|<span data-ttu-id="58c5e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58c5e-130">Type</span></span>|<span data-ttu-id="58c5e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58c5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c5e-132">domainName</span><span class="sxs-lookup"><span data-stu-id="58c5e-132">domainName</span></span>|<span data-ttu-id="58c5e-133">String</span><span class="sxs-lookup"><span data-stu-id="58c5e-133">String</span></span>|<span data-ttu-id="58c5e-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58c5e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="58c5e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="58c5e-135">Response</span></span>
<span data-ttu-id="58c5e-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58c5e-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58c5e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="58c5e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="58c5e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="58c5e-138">Request</span></span>
<span data-ttu-id="58c5e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58c5e-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="58c5e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="58c5e-140">Response</span></span>
<span data-ttu-id="58c5e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58c5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




