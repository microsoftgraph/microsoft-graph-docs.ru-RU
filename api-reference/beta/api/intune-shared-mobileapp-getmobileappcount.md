---
title: Функция getMobileAppCount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8cb917403ecb942d385506b5a382f8f23fe3fc3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729877"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="c1a95-103">Функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="c1a95-103">getMobileAppCount function</span></span>

<span data-ttu-id="c1a95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1a95-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1a95-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1a95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1a95-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c1a95-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1a95-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1a95-108">Prerequisites</span></span>
<span data-ttu-id="c1a95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a95-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a95-111">Permission type</span></span>|<span data-ttu-id="c1a95-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1a95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1a95-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1a95-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c1a95-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="c1a95-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c1a95-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1a95-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1a95-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1a95-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1a95-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a95-117">Not supported.</span></span>|
|<span data-ttu-id="c1a95-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1a95-118">Application</span></span>||
| <span data-ttu-id="c1a95-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="c1a95-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="c1a95-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1a95-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1a95-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1a95-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="c1a95-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1a95-122">Request headers</span></span>
|<span data-ttu-id="c1a95-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1a95-123">Header</span></span>|<span data-ttu-id="c1a95-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c1a95-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1a95-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1a95-125">Authorization</span></span>|<span data-ttu-id="c1a95-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a95-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1a95-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c1a95-127">Accept</span></span>|<span data-ttu-id="c1a95-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a95-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a95-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1a95-129">Request body</span></span>
<span data-ttu-id="c1a95-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c1a95-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c1a95-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c1a95-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c1a95-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1a95-132">Property</span></span>|<span data-ttu-id="c1a95-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c1a95-133">Type</span></span>|<span data-ttu-id="c1a95-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c1a95-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a95-135">status</span><span class="sxs-lookup"><span data-stu-id="c1a95-135">status</span></span>|<span data-ttu-id="c1a95-136">String</span><span class="sxs-lookup"><span data-stu-id="c1a95-136">String</span></span>|<span data-ttu-id="c1a95-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c1a95-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c1a95-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1a95-138">Response</span></span>
<span data-ttu-id="c1a95-139">В случае успеха эта функция возвращает `200 OK` код отклика и значение Int64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1a95-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a95-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c1a95-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1a95-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a95-141">Request</span></span>
<span data-ttu-id="c1a95-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a95-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c1a95-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a95-143">Response</span></span>
<span data-ttu-id="c1a95-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1a95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```








