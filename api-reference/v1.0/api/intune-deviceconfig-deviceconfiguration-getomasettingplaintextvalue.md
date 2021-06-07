---
title: функция getOmaSettingPlainTextValue
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4662cf110a95bfaf718e2d9ed0756d2329bcd996
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753450"
---
# <a name="getomasettingplaintextvalue-function"></a><span data-ttu-id="de462-103">функция getOmaSettingPlainTextValue</span><span class="sxs-lookup"><span data-stu-id="de462-103">getOmaSettingPlainTextValue function</span></span>

<span data-ttu-id="de462-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de462-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de462-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de462-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de462-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de462-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="de462-107">Prerequisites</span></span>
<span data-ttu-id="de462-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de462-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de462-110">Permission type</span></span>|<span data-ttu-id="de462-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de462-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de462-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de462-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de462-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de462-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de462-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de462-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de462-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de462-115">Not supported.</span></span>|
|<span data-ttu-id="de462-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="de462-116">Application</span></span>|<span data-ttu-id="de462-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de462-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de462-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de462-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue
```

## <a name="request-headers"></a><span data-ttu-id="de462-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de462-119">Request headers</span></span>
|<span data-ttu-id="de462-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de462-120">Header</span></span>|<span data-ttu-id="de462-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de462-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de462-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de462-122">Authorization</span></span>|<span data-ttu-id="de462-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de462-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de462-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de462-124">Accept</span></span>|<span data-ttu-id="de462-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de462-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de462-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de462-126">Request body</span></span>
<span data-ttu-id="de462-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="de462-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="de462-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="de462-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="de462-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="de462-129">Property</span></span>|<span data-ttu-id="de462-130">Тип</span><span class="sxs-lookup"><span data-stu-id="de462-130">Type</span></span>|<span data-ttu-id="de462-131">Описание</span><span class="sxs-lookup"><span data-stu-id="de462-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de462-132">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="de462-132">secretReferenceValueId</span></span>|<span data-ttu-id="de462-133">String</span><span class="sxs-lookup"><span data-stu-id="de462-133">String</span></span>|<span data-ttu-id="de462-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de462-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de462-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="de462-135">Response</span></span>
<span data-ttu-id="de462-136">В случае успешной работы эта функция возвращает код отклика и `200 OK` строку в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de462-136">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de462-137">Пример</span><span class="sxs-lookup"><span data-stu-id="de462-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="de462-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="de462-138">Request</span></span>
<span data-ttu-id="de462-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de462-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue(secretReferenceValueId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="de462-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="de462-140">Response</span></span>
<span data-ttu-id="de462-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de462-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": "Get Oma Setting Plain Text Value value"
}
```




