---
title: Получение Мобилеаппинтентандстате
description: Чтение свойств и связей объекта Мобилеаппинтентандстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26b0db271955c26ffdd58b5d4449d7f874cc787b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195372"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="bcdfa-103">Получение Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="bcdfa-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="bcdfa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcdfa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcdfa-106">Чтение свойств и связей объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bcdfa-106">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcdfa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcdfa-107">Prerequisites</span></span>
<span data-ttu-id="bcdfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcdfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcdfa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcdfa-110">Permission type</span></span>|<span data-ttu-id="bcdfa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcdfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcdfa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcdfa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcdfa-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcdfa-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bcdfa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcdfa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcdfa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-115">Not supported.</span></span>|
|<span data-ttu-id="bcdfa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcdfa-116">Application</span></span>|<span data-ttu-id="bcdfa-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcdfa-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcdfa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcdfa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcdfa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bcdfa-119">Optional query parameters</span></span>
<span data-ttu-id="bcdfa-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcdfa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcdfa-121">Request headers</span></span>
|<span data-ttu-id="bcdfa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcdfa-122">Header</span></span>|<span data-ttu-id="bcdfa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bcdfa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcdfa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcdfa-124">Authorization</span></span>|<span data-ttu-id="bcdfa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcdfa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bcdfa-126">Accept</span></span>|<span data-ttu-id="bcdfa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bcdfa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcdfa-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcdfa-128">Request body</span></span>
<span data-ttu-id="bcdfa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcdfa-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcdfa-130">Response</span></span>
<span data-ttu-id="bcdfa-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-131">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcdfa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bcdfa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcdfa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcdfa-133">Request</span></span>
<span data-ttu-id="bcdfa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="bcdfa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcdfa-135">Response</span></span>
<span data-ttu-id="bcdfa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcdfa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 943

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
    "id": "45a775d6-75d6-45a7-d675-a745d675a745",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "mobileAppList": [
      {
        "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
        "applicationId": "Application Id value",
        "displayName": "Display Name value",
        "mobileAppIntent": "notAvailable",
        "displayVersion": "Display Version value",
        "installState": "failed",
        "supportedDeviceTypes": [
          {
            "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
            "type": "windowsRT",
            "minimumOperatingSystemVersion": "Minimum Operating System Version value",
            "maximumOperatingSystemVersion": "Maximum Operating System Version value"
          }
        ]
      }
    ]
  }
}
```




