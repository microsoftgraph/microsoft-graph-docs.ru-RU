---
title: Функция Жетманажементкондитионстатементсфорплатформ
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd1b057616f106e169390e2aeb547480f7656a25
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696568"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="76ba5-103">Функция Жетманажементкондитионстатементсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="76ba5-103">getManagementConditionStatementsForPlatform function</span></span>

<span data-ttu-id="76ba5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76ba5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76ba5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ba5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76ba5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76ba5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76ba5-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="76ba5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76ba5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76ba5-108">Prerequisites</span></span>
<span data-ttu-id="76ba5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76ba5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76ba5-111">Permission type</span></span>|<span data-ttu-id="76ba5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76ba5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76ba5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76ba5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76ba5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76ba5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="76ba5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76ba5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76ba5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ba5-116">Not supported.</span></span>|
|<span data-ttu-id="76ba5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76ba5-117">Application</span></span>|<span data-ttu-id="76ba5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76ba5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76ba5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76ba5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="76ba5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76ba5-120">Request headers</span></span>
|<span data-ttu-id="76ba5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76ba5-121">Header</span></span>|<span data-ttu-id="76ba5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="76ba5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76ba5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76ba5-123">Authorization</span></span>|<span data-ttu-id="76ba5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76ba5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76ba5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76ba5-125">Accept</span></span>|<span data-ttu-id="76ba5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76ba5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76ba5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76ba5-127">Request body</span></span>
<span data-ttu-id="76ba5-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="76ba5-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="76ba5-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="76ba5-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="76ba5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76ba5-130">Property</span></span>|<span data-ttu-id="76ba5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76ba5-131">Type</span></span>|<span data-ttu-id="76ba5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76ba5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76ba5-133">платформа</span><span class="sxs-lookup"><span data-stu-id="76ba5-133">platform</span></span>|[<span data-ttu-id="76ba5-134">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="76ba5-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="76ba5-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="76ba5-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="76ba5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="76ba5-136">Response</span></span>
<span data-ttu-id="76ba5-137">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76ba5-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76ba5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="76ba5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="76ba5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="76ba5-139">Request</span></span>
<span data-ttu-id="76ba5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76ba5-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="76ba5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="76ba5-141">Response</span></span>
<span data-ttu-id="76ba5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76ba5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





