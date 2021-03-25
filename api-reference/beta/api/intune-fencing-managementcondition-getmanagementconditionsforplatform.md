---
title: функция getManagementConditionsForPlatform
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0b7d2f1ffdbe7dba4fbde09d80883fa60b5abaa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153736"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="de2f4-103">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="de2f4-103">getManagementConditionsForPlatform function</span></span>

<span data-ttu-id="de2f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de2f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de2f4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de2f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de2f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de2f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2f4-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de2f4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de2f4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="de2f4-108">Prerequisites</span></span>
<span data-ttu-id="de2f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de2f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de2f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de2f4-111">Permission type</span></span>|<span data-ttu-id="de2f4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de2f4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de2f4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de2f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de2f4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2f4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de2f4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de2f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de2f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de2f4-116">Not supported.</span></span>|
|<span data-ttu-id="de2f4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="de2f4-117">Application</span></span>|<span data-ttu-id="de2f4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2f4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de2f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de2f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="de2f4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de2f4-120">Request headers</span></span>
|<span data-ttu-id="de2f4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de2f4-121">Header</span></span>|<span data-ttu-id="de2f4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de2f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de2f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de2f4-123">Authorization</span></span>|<span data-ttu-id="de2f4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de2f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de2f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de2f4-125">Accept</span></span>|<span data-ttu-id="de2f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de2f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de2f4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de2f4-127">Request body</span></span>
<span data-ttu-id="de2f4-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="de2f4-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="de2f4-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="de2f4-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="de2f4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de2f4-130">Property</span></span>|<span data-ttu-id="de2f4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de2f4-131">Type</span></span>|<span data-ttu-id="de2f4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de2f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2f4-133">платформа</span><span class="sxs-lookup"><span data-stu-id="de2f4-133">platform</span></span>|[<span data-ttu-id="de2f4-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="de2f4-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="de2f4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="de2f4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de2f4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="de2f4-136">Response</span></span>
<span data-ttu-id="de2f4-137">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию managementCondition](../resources/intune-fencing-managementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de2f4-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de2f4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="de2f4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="de2f4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="de2f4-139">Request</span></span>
<span data-ttu-id="de2f4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de2f4-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="de2f4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="de2f4-141">Response</span></span>
<span data-ttu-id="de2f4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de2f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




