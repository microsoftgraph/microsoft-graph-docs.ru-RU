---
title: Получение Усерекспериенцеаналитиксбаселине
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксбаселине.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b712fc30400212d1330b024040faab1163523b24
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350494"
---
# <a name="get-userexperienceanalyticsbaseline"></a><span data-ttu-id="5a755-103">Получение Усерекспериенцеаналитиксбаселине</span><span class="sxs-lookup"><span data-stu-id="5a755-103">Get userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="5a755-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a755-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a755-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a755-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a755-106">Чтение свойств и связей объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="5a755-106">Read properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a755-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a755-107">Prerequisites</span></span>
<span data-ttu-id="5a755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a755-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a755-110">Permission type</span></span>|<span data-ttu-id="5a755-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a755-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a755-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a755-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a755-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a755-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5a755-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a755-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a755-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a755-115">Not supported.</span></span>|
|<span data-ttu-id="5a755-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a755-116">Application</span></span>|<span data-ttu-id="5a755-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a755-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a755-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a755-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a755-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5a755-119">Optional query parameters</span></span>
<span data-ttu-id="5a755-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5a755-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a755-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a755-121">Request headers</span></span>
|<span data-ttu-id="5a755-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a755-122">Header</span></span>|<span data-ttu-id="5a755-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5a755-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a755-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a755-124">Authorization</span></span>|<span data-ttu-id="5a755-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a755-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a755-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5a755-126">Accept</span></span>|<span data-ttu-id="5a755-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5a755-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a755-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a755-128">Request body</span></span>
<span data-ttu-id="5a755-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a755-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a755-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a755-130">Response</span></span>
<span data-ttu-id="5a755-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a755-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a755-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5a755-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a755-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a755-133">Request</span></span>
<span data-ttu-id="5a755-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a755-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

### <a name="response"></a><span data-ttu-id="5a755-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a755-135">Response</span></span>
<span data-ttu-id="5a755-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a755-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
    "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
    "displayName": "Display Name value",
    "overallScore": 12,
    "overallRegressionThreshold": 10
  }
}
```






