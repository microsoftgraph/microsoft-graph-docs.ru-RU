---
title: Получение Адванцедсреатпротектиононбоардингстатесуммари
description: Чтение свойств и связей объекта Адванцедсреатпротектиононбоардингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94e40e53a9e85c2c063e02b878bf6b7d66d85e40
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170282"
---
# <a name="get-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="e639d-103">Получение Адванцедсреатпротектиононбоардингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="e639d-103">Get advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="e639d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e639d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e639d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e639d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e639d-106">Чтение свойств и связей объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e639d-106">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e639d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e639d-107">Prerequisites</span></span>
<span data-ttu-id="e639d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e639d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e639d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e639d-110">Permission type</span></span>|<span data-ttu-id="e639d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e639d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e639d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e639d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e639d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e639d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e639d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e639d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e639d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e639d-115">Not supported.</span></span>|
|<span data-ttu-id="e639d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e639d-116">Application</span></span>|<span data-ttu-id="e639d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e639d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e639d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e639d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e639d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e639d-119">Optional query parameters</span></span>
<span data-ttu-id="e639d-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e639d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e639d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e639d-121">Request headers</span></span>
|<span data-ttu-id="e639d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e639d-122">Header</span></span>|<span data-ttu-id="e639d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e639d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e639d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e639d-124">Authorization</span></span>|<span data-ttu-id="e639d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e639d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e639d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e639d-126">Accept</span></span>|<span data-ttu-id="e639d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e639d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e639d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e639d-128">Request body</span></span>
<span data-ttu-id="e639d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e639d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e639d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e639d-130">Response</span></span>
<span data-ttu-id="e639d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e639d-131">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e639d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e639d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e639d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e639d-133">Request</span></span>
<span data-ttu-id="e639d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e639d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

### <a name="response"></a><span data-ttu-id="e639d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e639d-135">Response</span></span>
<span data-ttu-id="e639d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e639d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
    "id": "74089602-9602-7408-0296-087402960874",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3,
    "notAssignedDeviceCount": 6
  }
}
```




