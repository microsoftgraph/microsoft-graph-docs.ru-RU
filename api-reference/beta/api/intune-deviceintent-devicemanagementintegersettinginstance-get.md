---
title: Получение Девицеманажементинтежерсеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементинтежерсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3fade2afca558f62024ef441c3724e80e36cc82c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047723"
---
# <a name="get-devicemanagementintegersettinginstance"></a><span data-ttu-id="c2b12-103">Получение Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="c2b12-103">Get deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="c2b12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2b12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2b12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b12-107">Чтение свойств и связей объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="c2b12-107">Read properties and relationships of the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2b12-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2b12-108">Prerequisites</span></span>
<span data-ttu-id="c2b12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2b12-111">Permission type</span></span>|<span data-ttu-id="c2b12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2b12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2b12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2b12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2b12-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b12-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c2b12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2b12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2b12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b12-116">Not supported.</span></span>|
|<span data-ttu-id="c2b12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2b12-117">Application</span></span>|<span data-ttu-id="c2b12-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b12-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2b12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2b12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2b12-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2b12-120">Optional query parameters</span></span>
<span data-ttu-id="c2b12-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2b12-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2b12-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2b12-122">Request headers</span></span>
|<span data-ttu-id="c2b12-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2b12-123">Header</span></span>|<span data-ttu-id="c2b12-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c2b12-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2b12-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b12-125">Authorization</span></span>|<span data-ttu-id="c2b12-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2b12-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2b12-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c2b12-127">Accept</span></span>|<span data-ttu-id="c2b12-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b12-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2b12-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2b12-129">Request body</span></span>
<span data-ttu-id="c2b12-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2b12-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2b12-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b12-131">Response</span></span>
<span data-ttu-id="c2b12-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2b12-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2b12-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2b12-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2b12-134">Request</span></span>
<span data-ttu-id="c2b12-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2b12-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="c2b12-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b12-136">Response</span></span>
<span data-ttu-id="c2b12-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2b12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
    "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value",
    "value": 5
  }
}
```






