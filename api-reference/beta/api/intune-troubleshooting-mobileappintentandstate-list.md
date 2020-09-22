---
title: Список Мобилеаппинтентандстатес
description: Список свойств и связей объектов Мобилеаппинтентандстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ce16e8df84dc3f4fb73a79781c114a05100c53f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031828"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="5eb72-103">Список Мобилеаппинтентандстатес</span><span class="sxs-lookup"><span data-stu-id="5eb72-103">List mobileAppIntentAndStates</span></span>

<span data-ttu-id="5eb72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eb72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5eb72-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eb72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5eb72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5eb72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eb72-107">Список свойств и связей объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5eb72-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5eb72-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5eb72-108">Prerequisites</span></span>
<span data-ttu-id="5eb72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eb72-111">Permission type</span></span>|<span data-ttu-id="5eb72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eb72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eb72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eb72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5eb72-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5eb72-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5eb72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eb72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eb72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eb72-116">Not supported.</span></span>|
|<span data-ttu-id="5eb72-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eb72-117">Application</span></span>|<span data-ttu-id="5eb72-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5eb72-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eb72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eb72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="5eb72-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5eb72-120">Request headers</span></span>
|<span data-ttu-id="5eb72-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5eb72-121">Header</span></span>|<span data-ttu-id="5eb72-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5eb72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eb72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eb72-123">Authorization</span></span>|<span data-ttu-id="5eb72-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eb72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eb72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5eb72-125">Accept</span></span>|<span data-ttu-id="5eb72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5eb72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eb72-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5eb72-127">Request body</span></span>
<span data-ttu-id="5eb72-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5eb72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eb72-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eb72-129">Response</span></span>
<span data-ttu-id="5eb72-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5eb72-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eb72-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5eb72-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5eb72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eb72-132">Request</span></span>
<span data-ttu-id="5eb72-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eb72-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="5eb72-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eb72-134">Response</span></span>
<span data-ttu-id="5eb72-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5eb72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






