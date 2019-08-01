---
title: Получение объекта windowsInformationProtectionAppLearningSummary
description: Чтение свойств и связей объекта windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85b2c0a33a34ec9864fbd0b64baa5783bc0e6f03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023204"
---
# <a name="get-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="4cad3-103">Получение объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="4cad3-103">Get windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="4cad3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cad3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cad3-105">Чтение свойств и связей объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4cad3-105">Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cad3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4cad3-106">Prerequisites</span></span>
<span data-ttu-id="4cad3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cad3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cad3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cad3-109">Permission type</span></span>|<span data-ttu-id="4cad3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cad3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cad3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cad3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4cad3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cad3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4cad3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cad3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cad3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cad3-114">Not supported.</span></span>|
|<span data-ttu-id="4cad3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cad3-115">Application</span></span>|<span data-ttu-id="4cad3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cad3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cad3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cad3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cad3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cad3-118">Optional query parameters</span></span>
<span data-ttu-id="4cad3-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4cad3-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cad3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cad3-120">Request headers</span></span>
|<span data-ttu-id="4cad3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cad3-121">Header</span></span>|<span data-ttu-id="4cad3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4cad3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cad3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cad3-123">Authorization</span></span>|<span data-ttu-id="4cad3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cad3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cad3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cad3-125">Accept</span></span>|<span data-ttu-id="4cad3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cad3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cad3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cad3-127">Request body</span></span>
<span data-ttu-id="4cad3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cad3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cad3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cad3-129">Response</span></span>
<span data-ttu-id="4cad3-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4cad3-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cad3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4cad3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cad3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cad3-132">Request</span></span>
<span data-ttu-id="4cad3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cad3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="4cad3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cad3-134">Response</span></span>
<span data-ttu-id="4cad3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cad3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
    "id": "063baf50-af50-063b-50af-3b0650af3b06",
    "applicationName": "Application Name value",
    "applicationType": "desktop",
    "deviceCount": 11
  }
}
```



