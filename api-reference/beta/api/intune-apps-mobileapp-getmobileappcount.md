---
title: Функция getMobileAppCount
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be043b447e3b97bc248d62f25cdce19c906e81fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935366"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="d0c3b-103">Функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="d0c3b-103">getMobileAppCount function</span></span>

> <span data-ttu-id="d0c3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0c3b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0c3b-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0c3b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0c3b-107">Prerequisites</span></span>
<span data-ttu-id="d0c3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0c3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0c3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c3b-110">Permission type</span></span>|<span data-ttu-id="d0c3b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0c3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0c3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0c3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0c3b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0c3b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d0c3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0c3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0c3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-115">Not supported.</span></span>|
|<span data-ttu-id="d0c3b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0c3b-116">Application</span></span>|<span data-ttu-id="d0c3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0c3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0c3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="d0c3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0c3b-119">Request headers</span></span>
|<span data-ttu-id="d0c3b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0c3b-120">Header</span></span>|<span data-ttu-id="d0c3b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0c3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0c3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0c3b-122">Authorization</span></span>|<span data-ttu-id="d0c3b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0c3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d0c3b-124">Accept</span></span>|<span data-ttu-id="d0c3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0c3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0c3b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0c3b-126">Request body</span></span>
<span data-ttu-id="d0c3b-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d0c3b-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d0c3b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0c3b-129">Property</span></span>|<span data-ttu-id="d0c3b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c3b-130">Type</span></span>|<span data-ttu-id="d0c3b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0c3b-132">status</span><span class="sxs-lookup"><span data-stu-id="d0c3b-132">status</span></span>|<span data-ttu-id="d0c3b-133">String</span><span class="sxs-lookup"><span data-stu-id="d0c3b-133">String</span></span>|<span data-ttu-id="d0c3b-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0c3b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d0c3b-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0c3b-135">Response</span></span>
<span data-ttu-id="d0c3b-136">В случае успеха эта функция возвращает код `200 OK` отклика и значение Int64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-136">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c3b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d0c3b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0c3b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0c3b-138">Request</span></span>
<span data-ttu-id="d0c3b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d0c3b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c3b-140">Response</span></span>
<span data-ttu-id="d0c3b-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0c3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




