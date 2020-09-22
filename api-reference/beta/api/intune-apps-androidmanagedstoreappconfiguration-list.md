---
title: Список Андроидманажедстореаппконфигуратионс
description: Список свойств и связей объектов Андроидманажедстореаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8265e19ee664b586c24edc373a90dcd66c4b060b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006386"
---
# <a name="list-androidmanagedstoreappconfigurations"></a><span data-ttu-id="69f55-103">Список Андроидманажедстореаппконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="69f55-103">List androidManagedStoreAppConfigurations</span></span>

<span data-ttu-id="69f55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69f55-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69f55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f55-107">Список свойств и связей объектов [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="69f55-107">List properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f55-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69f55-108">Prerequisites</span></span>
<span data-ttu-id="69f55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f55-111">Permission type</span></span>|<span data-ttu-id="69f55-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69f55-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69f55-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="69f55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f55-116">Not supported.</span></span>|
|<span data-ttu-id="69f55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f55-117">Application</span></span>|<span data-ttu-id="69f55-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69f55-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="69f55-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69f55-120">Request headers</span></span>
|<span data-ttu-id="69f55-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f55-121">Header</span></span>|<span data-ttu-id="69f55-122">Значение</span><span class="sxs-lookup"><span data-stu-id="69f55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f55-123">Authorization</span></span>|<span data-ttu-id="69f55-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f55-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69f55-125">Accept</span></span>|<span data-ttu-id="69f55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69f55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f55-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69f55-127">Request body</span></span>
<span data-ttu-id="69f55-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69f55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f55-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f55-129">Response</span></span>
<span data-ttu-id="69f55-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69f55-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f55-131">Пример</span><span class="sxs-lookup"><span data-stu-id="69f55-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f55-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f55-132">Request</span></span>
<span data-ttu-id="69f55-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f55-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="69f55-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f55-134">Response</span></span>
<span data-ttu-id="69f55-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69f55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 942

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
      "id": "919a9335-9335-919a-3593-9a9135939a91",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "packageId": "Package Id value",
      "payloadJson": "Payload Json value",
      "permissionActions": [
        {
          "@odata.type": "microsoft.graph.androidPermissionAction",
          "permission": "Permission value",
          "action": "autoGrant"
        }
      ],
      "appSupportsOemConfig": true,
      "profileApplicability": "androidWorkProfile"
    }
  ]
}
```






