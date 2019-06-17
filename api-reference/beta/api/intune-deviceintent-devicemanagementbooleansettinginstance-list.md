---
title: Список Девицеманажементбулеансеттингинстанцес
description: Список свойств и связей объектов Девицеманажементбулеансеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 099027f076b54ac1665e4b2e03813a16422300e0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960939"
---
# <a name="list-devicemanagementbooleansettinginstances"></a><span data-ttu-id="1b029-103">Список Девицеманажементбулеансеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="1b029-103">List deviceManagementBooleanSettingInstances</span></span>

> <span data-ttu-id="1b029-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b029-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b029-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b029-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b029-106">Список свойств и связей объектов [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="1b029-106">List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b029-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b029-107">Prerequisites</span></span>
<span data-ttu-id="1b029-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b029-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b029-110">Permission type</span></span>|<span data-ttu-id="1b029-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b029-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b029-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b029-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b029-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b029-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1b029-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b029-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b029-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b029-115">Not supported.</span></span>|
|<span data-ttu-id="1b029-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b029-116">Application</span></span>|<span data-ttu-id="1b029-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b029-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b029-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b029-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1b029-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b029-119">Request headers</span></span>
|<span data-ttu-id="1b029-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b029-120">Header</span></span>|<span data-ttu-id="1b029-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b029-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b029-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b029-122">Authorization</span></span>|<span data-ttu-id="1b029-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b029-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b029-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b029-124">Accept</span></span>|<span data-ttu-id="1b029-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b029-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b029-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b029-126">Request body</span></span>
<span data-ttu-id="1b029-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b029-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b029-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b029-128">Response</span></span>
<span data-ttu-id="1b029-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b029-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b029-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1b029-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b029-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b029-131">Request</span></span>
<span data-ttu-id="1b029-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b029-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="1b029-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b029-133">Response</span></span>
<span data-ttu-id="1b029-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
      "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": true
    }
  ]
}
```





