---
title: Получение Мобилеаппинтентандстате
description: Чтение свойств и связей объекта Мобилеаппинтентандстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7eb62dd2ec2a19f08ae2e640ddf0703129ddae0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979283"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="620b3-103">Получение Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="620b3-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="620b3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="620b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="620b3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="620b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="620b3-106">Чтение свойств и связей объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="620b3-106">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="620b3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="620b3-107">Prerequisites</span></span>
<span data-ttu-id="620b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="620b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="620b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="620b3-110">Permission type</span></span>|<span data-ttu-id="620b3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="620b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="620b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="620b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="620b3-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="620b3-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="620b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="620b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="620b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="620b3-115">Not supported.</span></span>|
|<span data-ttu-id="620b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="620b3-116">Application</span></span>|<span data-ttu-id="620b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="620b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="620b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="620b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="620b3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="620b3-119">Optional query parameters</span></span>
<span data-ttu-id="620b3-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="620b3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="620b3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="620b3-121">Request headers</span></span>
|<span data-ttu-id="620b3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="620b3-122">Header</span></span>|<span data-ttu-id="620b3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="620b3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="620b3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="620b3-124">Authorization</span></span>|<span data-ttu-id="620b3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="620b3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="620b3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="620b3-126">Accept</span></span>|<span data-ttu-id="620b3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="620b3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="620b3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="620b3-128">Request body</span></span>
<span data-ttu-id="620b3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="620b3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="620b3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="620b3-130">Response</span></span>
<span data-ttu-id="620b3-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="620b3-131">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="620b3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="620b3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="620b3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="620b3-133">Request</span></span>
<span data-ttu-id="620b3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="620b3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="620b3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="620b3-135">Response</span></span>
<span data-ttu-id="620b3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="620b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





