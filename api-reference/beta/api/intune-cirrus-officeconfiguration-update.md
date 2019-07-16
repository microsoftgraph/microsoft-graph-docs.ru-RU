---
title: Обновление Оффицеконфигуратион
description: Обновление свойств объекта Оффицеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e452a3743148b4767c1259d68746924d3b0675c4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726134"
---
# <a name="update-officeconfiguration"></a><span data-ttu-id="2446b-103">Обновление Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2446b-103">Update officeConfiguration</span></span>

> <span data-ttu-id="2446b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2446b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2446b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2446b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2446b-106">Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2446b-106">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2446b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2446b-107">Prerequisites</span></span>
<span data-ttu-id="2446b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2446b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2446b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2446b-110">Permission type</span></span>|<span data-ttu-id="2446b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2446b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2446b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2446b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2446b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2446b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2446b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2446b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2446b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2446b-115">Not supported.</span></span>|
|<span data-ttu-id="2446b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2446b-116">Application</span></span>|<span data-ttu-id="2446b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2446b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2446b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2446b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="2446b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2446b-119">Request headers</span></span>
|<span data-ttu-id="2446b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2446b-120">Header</span></span>|<span data-ttu-id="2446b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2446b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2446b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2446b-122">Authorization</span></span>|<span data-ttu-id="2446b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2446b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2446b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2446b-124">Accept</span></span>|<span data-ttu-id="2446b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2446b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2446b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2446b-126">Request body</span></span>
<span data-ttu-id="2446b-127">В тексте запроса добавьте представление объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2446b-127">In the request body, supply a JSON representation for the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

<span data-ttu-id="2446b-128">В следующей таблице приведены свойства, необходимые при создании [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2446b-128">The following table shows the properties that are required when you create the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md).</span></span>

|<span data-ttu-id="2446b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2446b-129">Property</span></span>|<span data-ttu-id="2446b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2446b-130">Type</span></span>|<span data-ttu-id="2446b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2446b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2446b-132">id</span><span class="sxs-lookup"><span data-stu-id="2446b-132">id</span></span>|<span data-ttu-id="2446b-133">String</span><span class="sxs-lookup"><span data-stu-id="2446b-133">String</span></span>|<span data-ttu-id="2446b-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2446b-134">Not yet documented</span></span>|
|<span data-ttu-id="2446b-135">Тенантчеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="2446b-135">tenantCheckinStatuses</span></span>|<span data-ttu-id="2446b-136">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2446b-136">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="2446b-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2446b-137">Not yet documented</span></span>|
|<span data-ttu-id="2446b-138">Тенантусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="2446b-138">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="2446b-139">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="2446b-139">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="2446b-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2446b-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2446b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2446b-141">Response</span></span>
<span data-ttu-id="2446b-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2446b-142">If successful, this method returns a `200 OK` response code and an updated [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2446b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2446b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2446b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2446b-144">Request</span></span>
<span data-ttu-id="2446b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2446b-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration
Content-type: application/json
Content-length: 843

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```

### <a name="response"></a><span data-ttu-id="2446b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2446b-146">Response</span></span>
<span data-ttu-id="2446b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2446b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "4b5f7085-7085-4b5f-8570-5f4b85705f4b",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```





