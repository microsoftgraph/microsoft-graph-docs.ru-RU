---
title: Функция Ареглобалскриптсаваилабле
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afd259cc97b72863ac78dfdb1ab46e9f73bd02af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380974"
---
# <a name="areglobalscriptsavailable-function"></a><span data-ttu-id="aa981-103">Функция Ареглобалскриптсаваилабле</span><span class="sxs-lookup"><span data-stu-id="aa981-103">areGlobalScriptsAvailable function</span></span>

<span data-ttu-id="aa981-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa981-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa981-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa981-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa981-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa981-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa981-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aa981-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa981-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aa981-108">Prerequisites</span></span>
<span data-ttu-id="aa981-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa981-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa981-111">Permission type</span></span>|<span data-ttu-id="aa981-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa981-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa981-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa981-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa981-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa981-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aa981-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa981-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa981-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa981-116">Not supported.</span></span>|
|<span data-ttu-id="aa981-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="aa981-117">Application</span></span>|<span data-ttu-id="aa981-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa981-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa981-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa981-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/areGlobalScriptsAvailable
```

## <a name="request-headers"></a><span data-ttu-id="aa981-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa981-120">Request headers</span></span>
|<span data-ttu-id="aa981-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa981-121">Header</span></span>|<span data-ttu-id="aa981-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa981-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa981-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa981-123">Authorization</span></span>|<span data-ttu-id="aa981-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa981-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa981-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa981-125">Accept</span></span>|<span data-ttu-id="aa981-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa981-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa981-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa981-127">Request body</span></span>
<span data-ttu-id="aa981-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa981-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa981-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa981-129">Response</span></span>
<span data-ttu-id="aa981-130">В случае успеха эта функция возвращает код `200 OK` отклика и объект [глобалдевицехеалсскриптстате](../resources/intune-devices-globaldevicehealthscriptstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa981-130">If successful, this function returns a `200 OK` response code and a [globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa981-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa981-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa981-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa981-132">Request</span></span>
<span data-ttu-id="aa981-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa981-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/areGlobalScriptsAvailable
```

### <a name="response"></a><span data-ttu-id="aa981-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa981-134">Response</span></span>
<span data-ttu-id="aa981-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa981-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26

{
  "value": "pending"
}
```



