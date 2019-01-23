---
title: функция getManagementConditionsForPlatform
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2434d00c637112baa139ef92e4f77819ed8fd069
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420411"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="d89a2-103">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="d89a2-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="d89a2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d89a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d89a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d89a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d89a2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d89a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d89a2-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d89a2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d89a2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d89a2-108">Prerequisites</span></span>
<span data-ttu-id="d89a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d89a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d89a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d89a2-111">Permission type</span></span>|<span data-ttu-id="d89a2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d89a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d89a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d89a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d89a2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d89a2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d89a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d89a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d89a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d89a2-116">Not supported.</span></span>|
|<span data-ttu-id="d89a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d89a2-117">Application</span></span>|<span data-ttu-id="d89a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d89a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d89a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d89a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="d89a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d89a2-120">Request headers</span></span>
|<span data-ttu-id="d89a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d89a2-121">Header</span></span>|<span data-ttu-id="d89a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d89a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d89a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d89a2-123">Authorization</span></span>|<span data-ttu-id="d89a2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d89a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d89a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d89a2-125">Accept</span></span>|<span data-ttu-id="d89a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d89a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d89a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d89a2-127">Request body</span></span>
<span data-ttu-id="d89a2-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d89a2-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d89a2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="d89a2-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d89a2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d89a2-130">Property</span></span>|<span data-ttu-id="d89a2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d89a2-131">Type</span></span>|<span data-ttu-id="d89a2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d89a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d89a2-133">platform</span><span class="sxs-lookup"><span data-stu-id="d89a2-133">platform</span></span>|[<span data-ttu-id="d89a2-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d89a2-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d89a2-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d89a2-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d89a2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d89a2-136">Response</span></span>
<span data-ttu-id="d89a2-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [managementCondition](../resources/intune-fencing-managementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d89a2-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d89a2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d89a2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d89a2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d89a2-139">Request</span></span>
<span data-ttu-id="d89a2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d89a2-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d89a2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d89a2-141">Response</span></span>
<span data-ttu-id="d89a2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d89a2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




