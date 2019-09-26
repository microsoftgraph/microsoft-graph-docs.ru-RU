---
title: Получение Девицеманажементбулеансеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементбулеансеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93f1da7878ff323134b90d32a39143fa9cb553db
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186220"
---
# <a name="get-devicemanagementbooleansettinginstance"></a><span data-ttu-id="a2149-103">Получение Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="a2149-103">Get deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="a2149-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2149-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2149-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2149-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2149-106">Чтение свойств и связей объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="a2149-106">Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2149-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2149-107">Prerequisites</span></span>
<span data-ttu-id="a2149-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2149-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2149-110">Permission type</span></span>|<span data-ttu-id="a2149-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2149-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2149-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2149-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2149-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2149-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2149-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2149-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2149-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2149-115">Not supported.</span></span>|
|<span data-ttu-id="a2149-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2149-116">Application</span></span>|<span data-ttu-id="a2149-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2149-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2149-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2149-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="a2149-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2149-119">Optional query parameters</span></span>
<span data-ttu-id="a2149-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a2149-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2149-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2149-121">Request headers</span></span>
|<span data-ttu-id="a2149-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2149-122">Header</span></span>|<span data-ttu-id="a2149-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a2149-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2149-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2149-124">Authorization</span></span>|<span data-ttu-id="a2149-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2149-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2149-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a2149-126">Accept</span></span>|<span data-ttu-id="a2149-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a2149-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2149-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2149-128">Request body</span></span>
<span data-ttu-id="a2149-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2149-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2149-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2149-130">Response</span></span>
<span data-ttu-id="a2149-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2149-131">If successful, this method returns a `200 OK` response code and [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2149-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a2149-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2149-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2149-133">Request</span></span>
<span data-ttu-id="a2149-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2149-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="a2149-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2149-135">Response</span></span>
<span data-ttu-id="a2149-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2149-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




