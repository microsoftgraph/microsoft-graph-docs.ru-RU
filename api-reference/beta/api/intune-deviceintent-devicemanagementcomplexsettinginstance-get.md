---
title: Получение Девицеманажементкомплекссеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементкомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78253297cf6ba975b912e9b1eed15296fb14109e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49289785"
---
# <a name="get-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="41971-103">Получение Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="41971-103">Get deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="41971-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41971-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41971-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41971-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41971-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41971-107">Чтение свойств и связей объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="41971-107">Read properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41971-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="41971-108">Prerequisites</span></span>
<span data-ttu-id="41971-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41971-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41971-111">Permission type</span></span>|<span data-ttu-id="41971-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41971-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41971-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41971-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41971-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41971-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41971-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41971-116">Not supported.</span></span>|
|<span data-ttu-id="41971-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41971-117">Application</span></span>|<span data-ttu-id="41971-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41971-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41971-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41971-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="41971-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41971-120">Optional query parameters</span></span>
<span data-ttu-id="41971-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="41971-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41971-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41971-122">Request headers</span></span>
|<span data-ttu-id="41971-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41971-123">Header</span></span>|<span data-ttu-id="41971-124">Значение</span><span class="sxs-lookup"><span data-stu-id="41971-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41971-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41971-125">Authorization</span></span>|<span data-ttu-id="41971-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41971-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41971-127">Accept</span><span class="sxs-lookup"><span data-stu-id="41971-127">Accept</span></span>|<span data-ttu-id="41971-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41971-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41971-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41971-129">Request body</span></span>
<span data-ttu-id="41971-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41971-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41971-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="41971-131">Response</span></span>
<span data-ttu-id="41971-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41971-132">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41971-133">Пример</span><span class="sxs-lookup"><span data-stu-id="41971-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="41971-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="41971-134">Request</span></span>
<span data-ttu-id="41971-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41971-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="41971-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="41971-136">Response</span></span>
<span data-ttu-id="41971-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41971-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
    "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value"
  }
}
```




