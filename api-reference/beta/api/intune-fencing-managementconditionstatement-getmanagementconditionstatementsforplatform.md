---
title: функция getManagementConditionStatementsForPlatform
description: Н/Д
ms.openlocfilehash: d2855d7707cb8f1083f736c2a50d92e40e5d0278
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081315"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="4d36b-103">функция getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="4d36b-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="4d36b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d36b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d36b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d36b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d36b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d36b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d36b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d36b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d36b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4d36b-108">Prerequisites</span></span>
<span data-ttu-id="4d36b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d36b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d36b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d36b-111">Permission type</span></span>|<span data-ttu-id="4d36b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d36b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d36b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d36b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d36b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d36b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4d36b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d36b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d36b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d36b-116">Not supported.</span></span>|
|<span data-ttu-id="4d36b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d36b-117">Application</span></span>|<span data-ttu-id="4d36b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d36b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d36b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d36b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="4d36b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d36b-120">Request headers</span></span>
|<span data-ttu-id="4d36b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d36b-121">Header</span></span>|<span data-ttu-id="4d36b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4d36b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d36b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d36b-123">Authorization</span></span>|<span data-ttu-id="4d36b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4d36b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d36b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d36b-125">Accept</span></span>|<span data-ttu-id="4d36b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d36b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d36b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d36b-127">Request body</span></span>
<span data-ttu-id="4d36b-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="4d36b-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4d36b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4d36b-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4d36b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d36b-130">Property</span></span>|<span data-ttu-id="4d36b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4d36b-131">Type</span></span>|<span data-ttu-id="4d36b-132">Description</span><span class="sxs-lookup"><span data-stu-id="4d36b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d36b-133">platform</span><span class="sxs-lookup"><span data-stu-id="4d36b-133">platform</span></span>|[<span data-ttu-id="4d36b-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="4d36b-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="4d36b-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d36b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d36b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d36b-136">Response</span></span>
<span data-ttu-id="4d36b-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4d36b-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d36b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4d36b-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d36b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d36b-139">Request</span></span>
<span data-ttu-id="4d36b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d36b-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4d36b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d36b-141">Response</span></span>
<span data-ttu-id="4d36b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4d36b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

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
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





