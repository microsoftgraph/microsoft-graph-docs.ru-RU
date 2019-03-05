---
title: Функция Жетманажементкондитионсфорплатформ
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31eb739da3c29b95b77a9754045213d0abced3f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141547"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="618f5-103">Функция Жетманажементкондитионсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="618f5-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="618f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="618f5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="618f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="618f5-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="618f5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="618f5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="618f5-107">Prerequisites</span></span>
<span data-ttu-id="618f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="618f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="618f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="618f5-110">Permission type</span></span>|<span data-ttu-id="618f5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="618f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="618f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="618f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="618f5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="618f5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="618f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="618f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="618f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618f5-115">Not supported.</span></span>|
|<span data-ttu-id="618f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="618f5-116">Application</span></span>|<span data-ttu-id="618f5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="618f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="618f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="618f5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="618f5-119">Request headers</span></span>
|<span data-ttu-id="618f5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="618f5-120">Header</span></span>|<span data-ttu-id="618f5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="618f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="618f5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="618f5-122">Authorization</span></span>|<span data-ttu-id="618f5-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="618f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="618f5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="618f5-124">Accept</span></span>|<span data-ttu-id="618f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="618f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="618f5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="618f5-126">Request body</span></span>
<span data-ttu-id="618f5-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="618f5-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="618f5-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="618f5-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="618f5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="618f5-129">Property</span></span>|<span data-ttu-id="618f5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="618f5-130">Type</span></span>|<span data-ttu-id="618f5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="618f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="618f5-132">platform</span><span class="sxs-lookup"><span data-stu-id="618f5-132">platform</span></span>|[<span data-ttu-id="618f5-133">Девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="618f5-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="618f5-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="618f5-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="618f5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="618f5-135">Response</span></span>
<span data-ttu-id="618f5-136">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [манажементкондитион](../resources/intune-fencing-managementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="618f5-136">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="618f5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="618f5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="618f5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="618f5-138">Request</span></span>
<span data-ttu-id="618f5-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="618f5-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="618f5-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="618f5-140">Response</span></span>
<span data-ttu-id="618f5-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="618f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




