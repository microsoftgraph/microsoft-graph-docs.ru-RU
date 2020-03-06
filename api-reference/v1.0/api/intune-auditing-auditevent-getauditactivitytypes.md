---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1749bd523acd02cc39596906be9627604182f87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515751"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="93276-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="93276-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="93276-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93276-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93276-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93276-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93276-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="93276-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93276-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="93276-107">Prerequisites</span></span>
<span data-ttu-id="93276-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93276-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93276-110">Permission type</span></span>|<span data-ttu-id="93276-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93276-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93276-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93276-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93276-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="93276-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="93276-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93276-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93276-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93276-115">Not supported.</span></span>|
|<span data-ttu-id="93276-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93276-116">Application</span></span>|<span data-ttu-id="93276-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93276-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93276-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93276-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="93276-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93276-119">Request headers</span></span>
|<span data-ttu-id="93276-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93276-120">Header</span></span>|<span data-ttu-id="93276-121">Значение</span><span class="sxs-lookup"><span data-stu-id="93276-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93276-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93276-122">Authorization</span></span>|<span data-ttu-id="93276-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93276-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93276-124">Accept</span><span class="sxs-lookup"><span data-stu-id="93276-124">Accept</span></span>|<span data-ttu-id="93276-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93276-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93276-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93276-126">Request body</span></span>
<span data-ttu-id="93276-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="93276-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="93276-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="93276-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="93276-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="93276-129">Property</span></span>|<span data-ttu-id="93276-130">Тип</span><span class="sxs-lookup"><span data-stu-id="93276-130">Type</span></span>|<span data-ttu-id="93276-131">Описание</span><span class="sxs-lookup"><span data-stu-id="93276-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93276-132">category</span><span class="sxs-lookup"><span data-stu-id="93276-132">category</span></span>|<span data-ttu-id="93276-133">String</span><span class="sxs-lookup"><span data-stu-id="93276-133">String</span></span>|<span data-ttu-id="93276-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="93276-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="93276-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="93276-135">Response</span></span>
<span data-ttu-id="93276-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93276-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93276-137">Пример</span><span class="sxs-lookup"><span data-stu-id="93276-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="93276-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="93276-138">Request</span></span>
<span data-ttu-id="93276-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93276-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="93276-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="93276-140">Response</span></span>
<span data-ttu-id="93276-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93276-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




