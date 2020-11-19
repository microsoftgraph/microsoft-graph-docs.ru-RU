---
title: Функция Жетполицисуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1076a9870b62d069e3f4c572aef418c08e8f764
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302271"
---
# <a name="getpolicysummary-function"></a><span data-ttu-id="d13f9-103">Функция Жетполицисуммари</span><span class="sxs-lookup"><span data-stu-id="d13f9-103">getPolicySummary function</span></span>

<span data-ttu-id="d13f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d13f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d13f9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d13f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d13f9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d13f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d13f9-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d13f9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d13f9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d13f9-108">Prerequisites</span></span>
<span data-ttu-id="d13f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d13f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d13f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d13f9-111">Permission type</span></span>|<span data-ttu-id="d13f9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d13f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d13f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d13f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d13f9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d13f9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d13f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d13f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d13f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d13f9-116">Not supported.</span></span>|
|<span data-ttu-id="d13f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d13f9-117">Application</span></span>|<span data-ttu-id="d13f9-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d13f9-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d13f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d13f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections/getPolicySummary
```

## <a name="request-headers"></a><span data-ttu-id="d13f9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d13f9-120">Request headers</span></span>
|<span data-ttu-id="d13f9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d13f9-121">Header</span></span>|<span data-ttu-id="d13f9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d13f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d13f9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d13f9-123">Authorization</span></span>|<span data-ttu-id="d13f9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d13f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d13f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d13f9-125">Accept</span></span>|<span data-ttu-id="d13f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d13f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d13f9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d13f9-127">Request body</span></span>
<span data-ttu-id="d13f9-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d13f9-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d13f9-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="d13f9-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d13f9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d13f9-130">Property</span></span>|<span data-ttu-id="d13f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d13f9-131">Type</span></span>|<span data-ttu-id="d13f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d13f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d13f9-133">полициид</span><span class="sxs-lookup"><span data-stu-id="d13f9-133">policyId</span></span>|<span data-ttu-id="d13f9-134">String</span><span class="sxs-lookup"><span data-stu-id="d13f9-134">String</span></span>|<span data-ttu-id="d13f9-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d13f9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d13f9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d13f9-136">Response</span></span>
<span data-ttu-id="d13f9-137">В случае успеха эта функция возвращает `200 OK` код отклика и объект [конфигманажерполицисуммари](../resources/intune-partnerintegration-configmanagerpolicysummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d13f9-137">If successful, this function returns a `200 OK` response code and a [configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d13f9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d13f9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d13f9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d13f9-139">Request</span></span>
<span data-ttu-id="d13f9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d13f9-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections/getPolicySummary(policyId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d13f9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d13f9-141">Response</span></span>
<span data-ttu-id="d13f9-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d13f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": {
    "@odata.type": "microsoft.graph.configManagerPolicySummary",
    "targetedDeviceCount": 3,
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "failedDeviceCount": 1,
    "pendingDeviceCount": 2,
    "enforcedDeviceCount": 3
  }
}
```




