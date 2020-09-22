---
title: Получение Девицеманажементколлектионсеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементколлектионсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 282d599a546e97487dc953fa7aaaf8ebf5be33ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000744"
---
# <a name="get-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="60cdf-103">Получение Девицеманажементколлектионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="60cdf-103">Get deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="60cdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60cdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60cdf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60cdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60cdf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60cdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60cdf-107">Чтение свойств и связей объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="60cdf-107">Read properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60cdf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="60cdf-108">Prerequisites</span></span>
<span data-ttu-id="60cdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60cdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60cdf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60cdf-111">Permission type</span></span>|<span data-ttu-id="60cdf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="60cdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60cdf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60cdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60cdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="60cdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="60cdf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60cdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60cdf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60cdf-116">Not supported.</span></span>|
|<span data-ttu-id="60cdf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60cdf-117">Application</span></span>|<span data-ttu-id="60cdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="60cdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60cdf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60cdf-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="60cdf-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="60cdf-120">Optional query parameters</span></span>
<span data-ttu-id="60cdf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60cdf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60cdf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60cdf-122">Request headers</span></span>
|<span data-ttu-id="60cdf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60cdf-123">Header</span></span>|<span data-ttu-id="60cdf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="60cdf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60cdf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60cdf-125">Authorization</span></span>|<span data-ttu-id="60cdf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60cdf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60cdf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="60cdf-127">Accept</span></span>|<span data-ttu-id="60cdf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="60cdf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60cdf-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60cdf-129">Request body</span></span>
<span data-ttu-id="60cdf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60cdf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60cdf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="60cdf-131">Response</span></span>
<span data-ttu-id="60cdf-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60cdf-132">If successful, this method returns a `200 OK` response code and [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60cdf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="60cdf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="60cdf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="60cdf-134">Request</span></span>
<span data-ttu-id="60cdf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60cdf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="60cdf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="60cdf-136">Response</span></span>
<span data-ttu-id="60cdf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60cdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
    "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value"
  }
}
```






