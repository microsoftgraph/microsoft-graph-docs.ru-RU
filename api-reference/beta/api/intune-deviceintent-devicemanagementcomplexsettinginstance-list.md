---
title: Список Девицеманажементкомплекссеттингинстанцес
description: Список свойств и связей объектов Девицеманажементкомплекссеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da380a84be32958f62a8305550f0c7d6853b4609
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960638"
---
# <a name="list-devicemanagementcomplexsettinginstances"></a><span data-ttu-id="f9075-103">Список Девицеманажементкомплекссеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="f9075-103">List deviceManagementComplexSettingInstances</span></span>

> <span data-ttu-id="f9075-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9075-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9075-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9075-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9075-106">Список свойств и связей объектов [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="f9075-106">List properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9075-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9075-107">Prerequisites</span></span>
<span data-ttu-id="f9075-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9075-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9075-110">Permission type</span></span>|<span data-ttu-id="f9075-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9075-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9075-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9075-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9075-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9075-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f9075-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9075-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9075-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9075-115">Not supported.</span></span>|
|<span data-ttu-id="f9075-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9075-116">Application</span></span>|<span data-ttu-id="f9075-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9075-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9075-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9075-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="f9075-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9075-119">Request headers</span></span>
|<span data-ttu-id="f9075-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9075-120">Header</span></span>|<span data-ttu-id="f9075-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9075-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9075-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9075-122">Authorization</span></span>|<span data-ttu-id="f9075-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9075-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9075-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f9075-124">Accept</span></span>|<span data-ttu-id="f9075-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9075-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9075-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9075-126">Request body</span></span>
<span data-ttu-id="f9075-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9075-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9075-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9075-128">Response</span></span>
<span data-ttu-id="f9075-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9075-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9075-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f9075-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9075-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9075-131">Request</span></span>
<span data-ttu-id="f9075-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9075-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="f9075-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9075-133">Response</span></span>
<span data-ttu-id="f9075-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9075-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
      "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```





