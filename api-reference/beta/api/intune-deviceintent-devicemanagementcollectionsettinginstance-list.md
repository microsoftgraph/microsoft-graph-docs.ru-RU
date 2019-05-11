---
title: Список Девицеманажементколлектионсеттингинстанцес
description: Список свойств и связей объектов Девицеманажементколлектионсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d11981862aa77fa0271e4d5b081aec775eb09d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916666"
---
# <a name="list-devicemanagementcollectionsettinginstances"></a><span data-ttu-id="25035-103">Список Девицеманажементколлектионсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="25035-103">List deviceManagementCollectionSettingInstances</span></span>

> <span data-ttu-id="25035-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25035-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25035-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25035-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25035-106">Список свойств и связей объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="25035-106">List properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25035-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25035-107">Prerequisites</span></span>
<span data-ttu-id="25035-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25035-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25035-110">Permission type</span></span>|<span data-ttu-id="25035-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25035-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25035-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25035-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25035-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25035-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="25035-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25035-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25035-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25035-115">Not supported.</span></span>|
|<span data-ttu-id="25035-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25035-116">Application</span></span>|<span data-ttu-id="25035-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25035-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25035-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25035-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="25035-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25035-119">Request headers</span></span>
|<span data-ttu-id="25035-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25035-120">Header</span></span>|<span data-ttu-id="25035-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25035-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25035-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25035-122">Authorization</span></span>|<span data-ttu-id="25035-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25035-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25035-124">Accept</span><span class="sxs-lookup"><span data-stu-id="25035-124">Accept</span></span>|<span data-ttu-id="25035-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25035-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25035-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25035-126">Request body</span></span>
<span data-ttu-id="25035-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25035-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25035-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="25035-128">Response</span></span>
<span data-ttu-id="25035-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25035-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25035-130">Пример</span><span class="sxs-lookup"><span data-stu-id="25035-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="25035-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="25035-131">Request</span></span>
<span data-ttu-id="25035-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25035-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="25035-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="25035-133">Response</span></span>
<span data-ttu-id="25035-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25035-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
      "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```




