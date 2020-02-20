---
title: Функция Ареглобалскриптсаваилабле
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9da097cb1b3a9724605afb6bdbe0a25f4cf27aa
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162248"
---
# <a name="areglobalscriptsavailable-function"></a><span data-ttu-id="19ddf-103">Функция Ареглобалскриптсаваилабле</span><span class="sxs-lookup"><span data-stu-id="19ddf-103">areGlobalScriptsAvailable function</span></span>

> <span data-ttu-id="19ddf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19ddf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19ddf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19ddf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ddf-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="19ddf-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19ddf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19ddf-107">Prerequisites</span></span>
<span data-ttu-id="19ddf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19ddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ddf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19ddf-110">Permission type</span></span>|<span data-ttu-id="19ddf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19ddf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19ddf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19ddf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19ddf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ddf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="19ddf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19ddf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19ddf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19ddf-115">Not supported.</span></span>|
|<span data-ttu-id="19ddf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19ddf-116">Application</span></span>|<span data-ttu-id="19ddf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19ddf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19ddf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19ddf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/areGlobalScriptsAvailable
```

## <a name="request-headers"></a><span data-ttu-id="19ddf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="19ddf-119">Request headers</span></span>
|<span data-ttu-id="19ddf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19ddf-120">Header</span></span>|<span data-ttu-id="19ddf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19ddf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19ddf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ddf-122">Authorization</span></span>|<span data-ttu-id="19ddf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19ddf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19ddf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="19ddf-124">Accept</span></span>|<span data-ttu-id="19ddf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19ddf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ddf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19ddf-126">Request body</span></span>
<span data-ttu-id="19ddf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19ddf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19ddf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="19ddf-128">Response</span></span>
<span data-ttu-id="19ddf-129">В случае успеха эта функция возвращает код `200 OK` отклика и объект [глобалдевицехеалсскриптстате](../resources/intune-devices-globaldevicehealthscriptstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19ddf-129">If successful, this function returns a `200 OK` response code and a [globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ddf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="19ddf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="19ddf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="19ddf-131">Request</span></span>
<span data-ttu-id="19ddf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19ddf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/areGlobalScriptsAvailable
```

### <a name="response"></a><span data-ttu-id="19ddf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="19ddf-133">Response</span></span>
<span data-ttu-id="19ddf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19ddf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26

{
  "value": "pending"
}
```





