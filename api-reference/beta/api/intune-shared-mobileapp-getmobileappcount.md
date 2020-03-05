---
title: Функция getMobileAppCount
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b00e12a0810ba89ca868e6a1f4d9146ca351997
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458303"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="b1525-103">Функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="b1525-103">getMobileAppCount function</span></span>

<span data-ttu-id="b1525-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b1525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1525-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1525-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1525-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1525-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b1525-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1525-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1525-108">Prerequisites</span></span>
<span data-ttu-id="b1525-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1525-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1525-111">Permission type</span></span>|<span data-ttu-id="b1525-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1525-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1525-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1525-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b1525-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="b1525-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="b1525-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1525-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b1525-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1525-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1525-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1525-117">Not supported.</span></span>|
|<span data-ttu-id="b1525-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1525-118">Application</span></span>||
| <span data-ttu-id="b1525-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="b1525-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="b1525-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1525-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1525-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1525-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="b1525-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1525-122">Request headers</span></span>
|<span data-ttu-id="b1525-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1525-123">Header</span></span>|<span data-ttu-id="b1525-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b1525-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1525-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1525-125">Authorization</span></span>|<span data-ttu-id="b1525-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1525-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1525-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b1525-127">Accept</span></span>|<span data-ttu-id="b1525-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b1525-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1525-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1525-129">Request body</span></span>
<span data-ttu-id="b1525-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b1525-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b1525-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="b1525-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b1525-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1525-132">Property</span></span>|<span data-ttu-id="b1525-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b1525-133">Type</span></span>|<span data-ttu-id="b1525-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b1525-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1525-135">status</span><span class="sxs-lookup"><span data-stu-id="b1525-135">status</span></span>|<span data-ttu-id="b1525-136">String</span><span class="sxs-lookup"><span data-stu-id="b1525-136">String</span></span>|<span data-ttu-id="b1525-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b1525-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1525-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1525-138">Response</span></span>
<span data-ttu-id="b1525-139">В случае успеха эта функция возвращает код `200 OK` отклика и значение Int64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1525-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1525-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b1525-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1525-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1525-141">Request</span></span>
<span data-ttu-id="b1525-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1525-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b1525-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1525-143">Response</span></span>
<span data-ttu-id="b1525-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1525-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```








