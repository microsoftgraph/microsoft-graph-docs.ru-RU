---
title: Получение Девицеманажементкомплекссеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементкомплекссеттингинстанце.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89bb40c6b544a5f2f8146f9ea6efabf35dd210b0
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522309"
---
# <a name="get-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="7c5d2-103">Получение Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="7c5d2-103">Get deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="7c5d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c5d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c5d2-106">Чтение свойств и связей объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="7c5d2-106">Read properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c5d2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c5d2-107">Prerequisites</span></span>
<span data-ttu-id="7c5d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c5d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c5d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c5d2-110">Permission type</span></span>|<span data-ttu-id="7c5d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c5d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c5d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c5d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c5d2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c5d2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c5d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c5d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c5d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-115">Not supported.</span></span>|
|<span data-ttu-id="7c5d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c5d2-116">Application</span></span>|<span data-ttu-id="7c5d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c5d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c5d2-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="7c5d2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c5d2-119">Optional query parameters</span></span>
<span data-ttu-id="7c5d2-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c5d2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c5d2-121">Request headers</span></span>
|<span data-ttu-id="7c5d2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c5d2-122">Header</span></span>|<span data-ttu-id="7c5d2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7c5d2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c5d2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c5d2-124">Authorization</span></span>|<span data-ttu-id="7c5d2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c5d2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7c5d2-126">Accept</span></span>|<span data-ttu-id="7c5d2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c5d2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c5d2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c5d2-128">Request body</span></span>
<span data-ttu-id="7c5d2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c5d2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c5d2-130">Response</span></span>
<span data-ttu-id="7c5d2-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-131">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c5d2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7c5d2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c5d2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c5d2-133">Request</span></span>
<span data-ttu-id="7c5d2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="7c5d2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c5d2-135">Response</span></span>
<span data-ttu-id="7c5d2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c5d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







