---
title: Список Мобилеаппинтентандстатес
description: Список свойств и связей объектов Мобилеаппинтентандстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2391b5a5359ddf82dcef2106cd8ef46009107c9c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797776"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="d8546-103">Список Мобилеаппинтентандстатес</span><span class="sxs-lookup"><span data-stu-id="d8546-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="d8546-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8546-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8546-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8546-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8546-106">Список свойств и связей объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="d8546-106">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8546-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8546-107">Prerequisites</span></span>
<span data-ttu-id="d8546-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8546-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8546-110">Permission type</span></span>|<span data-ttu-id="d8546-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8546-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8546-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8546-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8546-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8546-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8546-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8546-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8546-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8546-115">Not supported.</span></span>|
|<span data-ttu-id="d8546-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8546-116">Application</span></span>|<span data-ttu-id="d8546-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8546-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8546-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8546-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="d8546-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8546-119">Request headers</span></span>
|<span data-ttu-id="d8546-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8546-120">Header</span></span>|<span data-ttu-id="d8546-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8546-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8546-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8546-122">Authorization</span></span>|<span data-ttu-id="d8546-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8546-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8546-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8546-124">Accept</span></span>|<span data-ttu-id="d8546-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8546-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8546-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8546-126">Request body</span></span>
<span data-ttu-id="d8546-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8546-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8546-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8546-128">Response</span></span>
<span data-ttu-id="d8546-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8546-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8546-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d8546-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8546-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8546-131">Request</span></span>
<span data-ttu-id="d8546-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8546-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="d8546-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8546-133">Response</span></span>
<span data-ttu-id="d8546-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8546-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



