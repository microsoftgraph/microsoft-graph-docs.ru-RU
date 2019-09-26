---
title: Функция getMobileAppCount
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80dff6cd579e7abd63bfcfb2eb76faee7771a972
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201164"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="8b659-103">Функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="8b659-103">getMobileAppCount function</span></span>

> <span data-ttu-id="8b659-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b659-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b659-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b659-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b659-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8b659-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b659-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b659-107">Prerequisites</span></span>
<span data-ttu-id="8b659-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b659-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b659-110">Permission type</span></span>|<span data-ttu-id="8b659-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b659-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b659-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b659-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8b659-113">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="8b659-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="8b659-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b659-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8b659-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b659-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b659-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b659-116">Not supported.</span></span>|
|<span data-ttu-id="8b659-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b659-117">Application</span></span>||
| <span data-ttu-id="8b659-118">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="8b659-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="8b659-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b659-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b659-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b659-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="8b659-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b659-121">Request headers</span></span>
|<span data-ttu-id="8b659-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b659-122">Header</span></span>|<span data-ttu-id="8b659-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8b659-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b659-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b659-124">Authorization</span></span>|<span data-ttu-id="8b659-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b659-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b659-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8b659-126">Accept</span></span>|<span data-ttu-id="8b659-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8b659-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b659-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b659-128">Request body</span></span>
<span data-ttu-id="8b659-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8b659-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8b659-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8b659-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8b659-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b659-131">Property</span></span>|<span data-ttu-id="8b659-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8b659-132">Type</span></span>|<span data-ttu-id="8b659-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8b659-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b659-134">status</span><span class="sxs-lookup"><span data-stu-id="8b659-134">status</span></span>|<span data-ttu-id="8b659-135">String</span><span class="sxs-lookup"><span data-stu-id="8b659-135">String</span></span>|<span data-ttu-id="8b659-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b659-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8b659-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b659-137">Response</span></span>
<span data-ttu-id="8b659-138">В случае успеха эта функция возвращает код `200 OK` отклика и значение Int64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b659-138">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b659-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8b659-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b659-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b659-140">Request</span></span>
<span data-ttu-id="8b659-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b659-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8b659-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b659-142">Response</span></span>
<span data-ttu-id="8b659-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b659-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




