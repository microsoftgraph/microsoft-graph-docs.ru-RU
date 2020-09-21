---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 845ae66814bbe02e52759e007bd58c749d5c3db3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966123"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="f7361-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="f7361-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="f7361-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7361-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7361-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7361-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7361-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7361-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7361-107">Prerequisites</span></span>
<span data-ttu-id="f7361-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7361-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7361-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7361-110">Permission type</span></span>|<span data-ttu-id="f7361-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7361-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7361-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7361-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7361-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7361-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f7361-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7361-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7361-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7361-115">Not supported.</span></span>|
|<span data-ttu-id="f7361-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7361-116">Application</span></span>|<span data-ttu-id="f7361-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7361-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7361-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7361-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="f7361-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7361-119">Request headers</span></span>
|<span data-ttu-id="f7361-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7361-120">Header</span></span>|<span data-ttu-id="f7361-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f7361-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7361-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7361-122">Authorization</span></span>|<span data-ttu-id="f7361-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7361-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7361-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f7361-124">Accept</span></span>|<span data-ttu-id="f7361-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7361-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7361-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7361-126">Request body</span></span>
<span data-ttu-id="f7361-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f7361-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f7361-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="f7361-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f7361-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7361-129">Property</span></span>|<span data-ttu-id="f7361-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f7361-130">Type</span></span>|<span data-ttu-id="f7361-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f7361-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7361-132">category</span><span class="sxs-lookup"><span data-stu-id="f7361-132">category</span></span>|<span data-ttu-id="f7361-133">String</span><span class="sxs-lookup"><span data-stu-id="f7361-133">String</span></span>|<span data-ttu-id="f7361-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7361-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7361-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7361-135">Response</span></span>
<span data-ttu-id="f7361-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7361-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7361-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f7361-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7361-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7361-138">Request</span></span>
<span data-ttu-id="f7361-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7361-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f7361-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7361-140">Response</span></span>
<span data-ttu-id="f7361-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7361-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```









