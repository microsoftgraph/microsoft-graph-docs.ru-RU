---
title: Получение Девицеманажементбулеансеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементбулеансеттингинстанце.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c1766b08bf652fc0294cddd4789bcf19bc61ceb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731077"
---
# <a name="get-devicemanagementbooleansettinginstance"></a><span data-ttu-id="34a49-103">Получение Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="34a49-103">Get deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="34a49-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34a49-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34a49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a49-106">Чтение свойств и связей объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="34a49-106">Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34a49-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34a49-107">Prerequisites</span></span>
<span data-ttu-id="34a49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a49-110">Permission type</span></span>|<span data-ttu-id="34a49-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34a49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34a49-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a49-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34a49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a49-115">Not supported.</span></span>|
|<span data-ttu-id="34a49-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="34a49-116">Application</span></span>|<span data-ttu-id="34a49-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a49-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34a49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34a49-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="34a49-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34a49-119">Optional query parameters</span></span>
<span data-ttu-id="34a49-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="34a49-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34a49-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34a49-121">Request headers</span></span>
|<span data-ttu-id="34a49-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34a49-122">Header</span></span>|<span data-ttu-id="34a49-123">Значение</span><span class="sxs-lookup"><span data-stu-id="34a49-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34a49-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a49-124">Authorization</span></span>|<span data-ttu-id="34a49-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a49-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34a49-126">Accept</span><span class="sxs-lookup"><span data-stu-id="34a49-126">Accept</span></span>|<span data-ttu-id="34a49-127">application/json</span><span class="sxs-lookup"><span data-stu-id="34a49-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a49-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34a49-128">Request body</span></span>
<span data-ttu-id="34a49-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34a49-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34a49-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="34a49-130">Response</span></span>
<span data-ttu-id="34a49-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34a49-131">If successful, this method returns a `200 OK` response code and [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a49-132">Пример</span><span class="sxs-lookup"><span data-stu-id="34a49-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a49-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="34a49-133">Request</span></span>
<span data-ttu-id="34a49-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34a49-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="34a49-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a49-135">Response</span></span>
<span data-ttu-id="34a49-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34a49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 254

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
    "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value",
    "value": true
  }
}
```




