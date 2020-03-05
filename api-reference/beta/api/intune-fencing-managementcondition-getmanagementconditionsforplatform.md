---
title: Функция Жетманажементкондитионсфорплатформ
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d63e0c3f3775b2b9999d364fcc79dad6adedf98f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465830"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="9120f-103">Функция Жетманажементкондитионсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="9120f-103">getManagementConditionsForPlatform function</span></span>

<span data-ttu-id="9120f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9120f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9120f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9120f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9120f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9120f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9120f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9120f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9120f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9120f-108">Prerequisites</span></span>
<span data-ttu-id="9120f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9120f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9120f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9120f-111">Permission type</span></span>|<span data-ttu-id="9120f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9120f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9120f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9120f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9120f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9120f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9120f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9120f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9120f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9120f-116">Not supported.</span></span>|
|<span data-ttu-id="9120f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9120f-117">Application</span></span>|<span data-ttu-id="9120f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9120f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9120f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9120f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="9120f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9120f-120">Request headers</span></span>
|<span data-ttu-id="9120f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9120f-121">Header</span></span>|<span data-ttu-id="9120f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9120f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9120f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9120f-123">Authorization</span></span>|<span data-ttu-id="9120f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9120f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9120f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9120f-125">Accept</span></span>|<span data-ttu-id="9120f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9120f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9120f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9120f-127">Request body</span></span>
<span data-ttu-id="9120f-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="9120f-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9120f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="9120f-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9120f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9120f-130">Property</span></span>|<span data-ttu-id="9120f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9120f-131">Type</span></span>|<span data-ttu-id="9120f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9120f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9120f-133">platform</span><span class="sxs-lookup"><span data-stu-id="9120f-133">platform</span></span>|[<span data-ttu-id="9120f-134">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="9120f-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="9120f-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9120f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9120f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9120f-136">Response</span></span>
<span data-ttu-id="9120f-137">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [манажементкондитион](../resources/intune-fencing-managementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9120f-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9120f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9120f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9120f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9120f-139">Request</span></span>
<span data-ttu-id="9120f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9120f-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9120f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9120f-141">Response</span></span>
<span data-ttu-id="9120f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9120f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





