---
title: функция getManagementConditionStatementsForPlatform
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1158b4f6b804ab7e852cab1d8a46cb4818599f21
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153617"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="2a88e-103">функция getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="2a88e-103">getManagementConditionStatementsForPlatform function</span></span>

<span data-ttu-id="2a88e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a88e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a88e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a88e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a88e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a88e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a88e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2a88e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a88e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a88e-108">Prerequisites</span></span>
<span data-ttu-id="2a88e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a88e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a88e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a88e-111">Permission type</span></span>|<span data-ttu-id="2a88e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a88e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a88e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a88e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a88e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a88e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a88e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a88e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a88e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a88e-116">Not supported.</span></span>|
|<span data-ttu-id="2a88e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a88e-117">Application</span></span>|<span data-ttu-id="2a88e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a88e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a88e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a88e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="2a88e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a88e-120">Request headers</span></span>
|<span data-ttu-id="2a88e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a88e-121">Header</span></span>|<span data-ttu-id="2a88e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2a88e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a88e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a88e-123">Authorization</span></span>|<span data-ttu-id="2a88e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a88e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a88e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a88e-125">Accept</span></span>|<span data-ttu-id="2a88e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a88e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a88e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a88e-127">Request body</span></span>
<span data-ttu-id="2a88e-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="2a88e-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2a88e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="2a88e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2a88e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a88e-130">Property</span></span>|<span data-ttu-id="2a88e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2a88e-131">Type</span></span>|<span data-ttu-id="2a88e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2a88e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a88e-133">платформа</span><span class="sxs-lookup"><span data-stu-id="2a88e-133">platform</span></span>|[<span data-ttu-id="2a88e-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="2a88e-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="2a88e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2a88e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2a88e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a88e-136">Response</span></span>
<span data-ttu-id="2a88e-137">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a88e-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a88e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2a88e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a88e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a88e-139">Request</span></span>
<span data-ttu-id="2a88e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a88e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2a88e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a88e-141">Response</span></span>
<span data-ttu-id="2a88e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a88e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpressionString",
        "value": "Value value"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




