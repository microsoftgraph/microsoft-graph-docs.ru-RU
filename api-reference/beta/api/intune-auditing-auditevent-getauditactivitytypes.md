---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c730a5154cbd9b8ab23572fbf9950077c6824abd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975908"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="f6e5e-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="f6e5e-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="f6e5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6e5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6e5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6e5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6e5e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6e5e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6e5e-108">Prerequisites</span></span>
<span data-ttu-id="f6e5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6e5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6e5e-111">Permission type</span></span>|<span data-ttu-id="f6e5e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6e5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6e5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6e5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6e5e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6e5e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f6e5e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6e5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6e5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-116">Not supported.</span></span>|
|<span data-ttu-id="f6e5e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6e5e-117">Application</span></span>|<span data-ttu-id="f6e5e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6e5e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6e5e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6e5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="f6e5e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6e5e-120">Request headers</span></span>
|<span data-ttu-id="f6e5e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6e5e-121">Header</span></span>|<span data-ttu-id="f6e5e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6e5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6e5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6e5e-123">Authorization</span></span>|<span data-ttu-id="f6e5e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6e5e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6e5e-125">Accept</span></span>|<span data-ttu-id="f6e5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6e5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6e5e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6e5e-127">Request body</span></span>
<span data-ttu-id="f6e5e-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f6e5e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f6e5e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6e5e-130">Property</span></span>|<span data-ttu-id="f6e5e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6e5e-131">Type</span></span>|<span data-ttu-id="f6e5e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6e5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e5e-133">category</span><span class="sxs-lookup"><span data-stu-id="f6e5e-133">category</span></span>|<span data-ttu-id="f6e5e-134">String</span><span class="sxs-lookup"><span data-stu-id="f6e5e-134">String</span></span>|<span data-ttu-id="f6e5e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f6e5e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6e5e-136">Response</span></span>
<span data-ttu-id="f6e5e-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6e5e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f6e5e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6e5e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6e5e-139">Request</span></span>
<span data-ttu-id="f6e5e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f6e5e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6e5e-141">Response</span></span>
<span data-ttu-id="f6e5e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






