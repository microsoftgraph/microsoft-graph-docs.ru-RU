---
title: Список Девицеманажементтемплатес
description: Список свойств и связей объектов Девицеманажементтемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3875ab5fc76c4b2d8c9968004f8201ad7508c119
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532066"
---
# <a name="list-devicemanagementtemplates"></a><span data-ttu-id="f42fb-103">Список Девицеманажементтемплатес</span><span class="sxs-lookup"><span data-stu-id="f42fb-103">List deviceManagementTemplates</span></span>

> <span data-ttu-id="f42fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f42fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f42fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f42fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f42fb-106">Список свойств и связей объектов [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="f42fb-106">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f42fb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f42fb-107">Prerequisites</span></span>
<span data-ttu-id="f42fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f42fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f42fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f42fb-110">Permission type</span></span>|<span data-ttu-id="f42fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f42fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f42fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f42fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f42fb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f42fb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f42fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f42fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f42fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f42fb-115">Not supported.</span></span>|
|<span data-ttu-id="f42fb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f42fb-116">Application</span></span>|<span data-ttu-id="f42fb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f42fb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f42fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f42fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="f42fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f42fb-119">Request headers</span></span>
|<span data-ttu-id="f42fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f42fb-120">Header</span></span>|<span data-ttu-id="f42fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f42fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f42fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f42fb-122">Authorization</span></span>|<span data-ttu-id="f42fb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f42fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f42fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f42fb-124">Accept</span></span>|<span data-ttu-id="f42fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f42fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f42fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f42fb-126">Request body</span></span>
<span data-ttu-id="f42fb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f42fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f42fb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f42fb-128">Response</span></span>
<span data-ttu-id="f42fb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f42fb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f42fb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f42fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f42fb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f42fb-131">Request</span></span>
<span data-ttu-id="f42fb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f42fb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="f42fb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f42fb-133">Response</span></span>
<span data-ttu-id="f42fb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f42fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 493

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplate",
      "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "specializedDevices",
      "platformType": "androidForWork",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
    }
  ]
}
```






