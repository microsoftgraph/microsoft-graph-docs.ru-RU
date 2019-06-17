---
title: Список Мобилеаппинтентандстатес
description: Список свойств и связей объектов Мобилеаппинтентандстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db30c5a04abc03a599f8a41c1f0c2b9ab9a33fbf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990710"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="27d8f-103">Список Мобилеаппинтентандстатес</span><span class="sxs-lookup"><span data-stu-id="27d8f-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="27d8f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27d8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27d8f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27d8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27d8f-106">Список свойств и связей объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="27d8f-106">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27d8f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27d8f-107">Prerequisites</span></span>
<span data-ttu-id="27d8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27d8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27d8f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27d8f-110">Permission type</span></span>|<span data-ttu-id="27d8f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27d8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27d8f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27d8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27d8f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="27d8f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="27d8f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27d8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27d8f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27d8f-115">Not supported.</span></span>|
|<span data-ttu-id="27d8f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27d8f-116">Application</span></span>|<span data-ttu-id="27d8f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27d8f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27d8f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27d8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="27d8f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27d8f-119">Request headers</span></span>
|<span data-ttu-id="27d8f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27d8f-120">Header</span></span>|<span data-ttu-id="27d8f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="27d8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27d8f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27d8f-122">Authorization</span></span>|<span data-ttu-id="27d8f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27d8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27d8f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="27d8f-124">Accept</span></span>|<span data-ttu-id="27d8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27d8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27d8f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27d8f-126">Request body</span></span>
<span data-ttu-id="27d8f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27d8f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27d8f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="27d8f-128">Response</span></span>
<span data-ttu-id="27d8f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27d8f-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27d8f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="27d8f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="27d8f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="27d8f-131">Request</span></span>
<span data-ttu-id="27d8f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27d8f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="27d8f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="27d8f-133">Response</span></span>
<span data-ttu-id="27d8f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27d8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
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
  ]
}
```





