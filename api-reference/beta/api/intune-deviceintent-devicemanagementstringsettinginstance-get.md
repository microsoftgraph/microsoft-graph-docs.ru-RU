---
title: Get deviceManagementStringSettingInstance
description: Чтение свойств и связей объекта deviceManagementStringSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26484f72c8677414cdf249c6f75335dc5f45c2f8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150768"
---
# <a name="get-devicemanagementstringsettinginstance"></a><span data-ttu-id="deecf-103">Get deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="deecf-103">Get deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="deecf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deecf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="deecf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deecf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="deecf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="deecf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deecf-107">Чтение свойств и связей [объекта deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="deecf-107">Read properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deecf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="deecf-108">Prerequisites</span></span>
<span data-ttu-id="deecf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deecf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deecf-111">Permission type</span></span>|<span data-ttu-id="deecf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deecf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deecf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deecf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="deecf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deecf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="deecf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deecf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deecf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deecf-116">Not supported.</span></span>|
|<span data-ttu-id="deecf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="deecf-117">Application</span></span>|<span data-ttu-id="deecf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deecf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="deecf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deecf-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="deecf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="deecf-120">Optional query parameters</span></span>
<span data-ttu-id="deecf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="deecf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deecf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deecf-122">Request headers</span></span>
|<span data-ttu-id="deecf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="deecf-123">Header</span></span>|<span data-ttu-id="deecf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="deecf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deecf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="deecf-125">Authorization</span></span>|<span data-ttu-id="deecf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deecf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deecf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="deecf-127">Accept</span></span>|<span data-ttu-id="deecf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="deecf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deecf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deecf-129">Request body</span></span>
<span data-ttu-id="deecf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="deecf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deecf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="deecf-131">Response</span></span>
<span data-ttu-id="deecf-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="deecf-132">If successful, this method returns a `200 OK` response code and [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deecf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="deecf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="deecf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="deecf-134">Request</span></span>
<span data-ttu-id="deecf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deecf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="deecf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="deecf-136">Response</span></span>
<span data-ttu-id="deecf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="deecf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
    "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value",
    "value": "Value value"
  }
}
```




