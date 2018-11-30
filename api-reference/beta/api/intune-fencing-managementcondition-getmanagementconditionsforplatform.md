---
title: функция getManagementConditionsForPlatform
description: Н/Д
ms.openlocfilehash: fd2de51131a2b4a6b125bfe935bce5c2cfc93fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080468"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="8002a-103">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="8002a-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="8002a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8002a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8002a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8002a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8002a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8002a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8002a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8002a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8002a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8002a-108">Prerequisites</span></span>
<span data-ttu-id="8002a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8002a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8002a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8002a-111">Permission type</span></span>|<span data-ttu-id="8002a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8002a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8002a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8002a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8002a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8002a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8002a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8002a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8002a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8002a-116">Not supported.</span></span>|
|<span data-ttu-id="8002a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8002a-117">Application</span></span>|<span data-ttu-id="8002a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8002a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8002a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8002a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="8002a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8002a-120">Request headers</span></span>
|<span data-ttu-id="8002a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8002a-121">Header</span></span>|<span data-ttu-id="8002a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8002a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8002a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8002a-123">Authorization</span></span>|<span data-ttu-id="8002a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8002a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8002a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8002a-125">Accept</span></span>|<span data-ttu-id="8002a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8002a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8002a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8002a-127">Request body</span></span>
<span data-ttu-id="8002a-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8002a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8002a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8002a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8002a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8002a-130">Property</span></span>|<span data-ttu-id="8002a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8002a-131">Type</span></span>|<span data-ttu-id="8002a-132">Description</span><span class="sxs-lookup"><span data-stu-id="8002a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8002a-133">platform</span><span class="sxs-lookup"><span data-stu-id="8002a-133">platform</span></span>|[<span data-ttu-id="8002a-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="8002a-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="8002a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8002a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8002a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8002a-136">Response</span></span>
<span data-ttu-id="8002a-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [managementCondition](../resources/intune-fencing-managementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8002a-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8002a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8002a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="8002a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8002a-139">Request</span></span>
<span data-ttu-id="8002a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8002a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8002a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="8002a-141">Response</span></span>
<span data-ttu-id="8002a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8002a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





