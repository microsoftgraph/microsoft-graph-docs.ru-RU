---
title: Список объектов windowsInformationProtectionAppLearningSummary
description: Список свойств и связей объектов windowsInformationProtectionAppLearningSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3353785d562bc4d2f613804d751330f06d579c4f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360974"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="8f890-103">Список объектов windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="8f890-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="8f890-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f890-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f890-105">Список свойств и связей объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="8f890-105">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f890-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8f890-106">Prerequisites</span></span>
<span data-ttu-id="8f890-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f890-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f890-109">Permission type</span></span>|<span data-ttu-id="8f890-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f890-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f890-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f890-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f890-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f890-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f890-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f890-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f890-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f890-114">Not supported.</span></span>|
|<span data-ttu-id="8f890-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f890-115">Application</span></span>|<span data-ttu-id="8f890-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f890-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f890-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f890-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="8f890-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f890-118">Request headers</span></span>
|<span data-ttu-id="8f890-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f890-119">Header</span></span>|<span data-ttu-id="8f890-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8f890-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f890-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f890-121">Authorization</span></span>|<span data-ttu-id="8f890-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f890-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f890-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8f890-123">Accept</span></span>|<span data-ttu-id="8f890-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f890-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f890-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f890-125">Request body</span></span>
<span data-ttu-id="8f890-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f890-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f890-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f890-127">Response</span></span>
<span data-ttu-id="8f890-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f890-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f890-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8f890-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f890-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f890-130">Request</span></span>
<span data-ttu-id="8f890-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f890-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="8f890-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f890-132">Response</span></span>
<span data-ttu-id="8f890-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f890-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
      "id": "063baf50-af50-063b-50af-3b0650af3b06",
      "applicationName": "Application Name value",
      "applicationType": "desktop",
      "deviceCount": 11
    }
  ]
}
```




