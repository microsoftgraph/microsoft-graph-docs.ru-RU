---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11d4027fbbcb1784663531bc9a15fbeaeec73824
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444625"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="1d0cf-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="1d0cf-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="1d0cf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d0cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d0cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d0cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d0cf-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d0cf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1d0cf-108">Prerequisites</span></span>
<span data-ttu-id="1d0cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d0cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d0cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d0cf-111">Permission type</span></span>|<span data-ttu-id="1d0cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d0cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d0cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d0cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d0cf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d0cf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1d0cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d0cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d0cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-116">Not supported.</span></span>|
|<span data-ttu-id="1d0cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d0cf-117">Application</span></span>|<span data-ttu-id="1d0cf-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d0cf-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d0cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d0cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="1d0cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1d0cf-120">Request headers</span></span>
|<span data-ttu-id="1d0cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d0cf-121">Header</span></span>|<span data-ttu-id="1d0cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d0cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d0cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d0cf-123">Authorization</span></span>|<span data-ttu-id="1d0cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d0cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d0cf-125">Accept</span></span>|<span data-ttu-id="1d0cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d0cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d0cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d0cf-127">Request body</span></span>
<span data-ttu-id="1d0cf-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1d0cf-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1d0cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d0cf-130">Property</span></span>|<span data-ttu-id="1d0cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1d0cf-131">Type</span></span>|<span data-ttu-id="1d0cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1d0cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d0cf-133">category</span><span class="sxs-lookup"><span data-stu-id="1d0cf-133">category</span></span>|<span data-ttu-id="1d0cf-134">String</span><span class="sxs-lookup"><span data-stu-id="1d0cf-134">String</span></span>|<span data-ttu-id="1d0cf-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d0cf-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1d0cf-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d0cf-136">Response</span></span>
<span data-ttu-id="1d0cf-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d0cf-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1d0cf-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d0cf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d0cf-139">Request</span></span>
<span data-ttu-id="1d0cf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1d0cf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d0cf-141">Response</span></span>
<span data-ttu-id="1d0cf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d0cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





