---
title: Список Андроидфорворкмобилеаппконфигуратионс
description: Список свойств и связей объектов Андроидфорворкмобилеаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f5a10a0c7c30ac075119fb963e2c9e91ab409da9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700782"
---
# <a name="list-androidforworkmobileappconfigurations"></a><span data-ttu-id="fa33d-103">Список Андроидфорворкмобилеаппконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="fa33d-103">List androidForWorkMobileAppConfigurations</span></span>

<span data-ttu-id="fa33d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa33d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa33d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa33d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa33d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa33d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa33d-107">Список свойств и связей объектов [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fa33d-107">List properties and relationships of the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa33d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa33d-108">Prerequisites</span></span>
<span data-ttu-id="fa33d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa33d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa33d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa33d-111">Permission type</span></span>|<span data-ttu-id="fa33d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa33d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa33d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa33d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa33d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa33d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa33d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa33d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa33d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa33d-116">Not supported.</span></span>|
|<span data-ttu-id="fa33d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa33d-117">Application</span></span>|<span data-ttu-id="fa33d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa33d-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa33d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa33d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa33d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa33d-120">Request headers</span></span>
|<span data-ttu-id="fa33d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa33d-121">Header</span></span>|<span data-ttu-id="fa33d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa33d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa33d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa33d-123">Authorization</span></span>|<span data-ttu-id="fa33d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa33d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa33d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa33d-125">Accept</span></span>|<span data-ttu-id="fa33d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa33d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa33d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa33d-127">Request body</span></span>
<span data-ttu-id="fa33d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa33d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa33d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa33d-129">Response</span></span>
<span data-ttu-id="fa33d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa33d-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa33d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fa33d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa33d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa33d-132">Request</span></span>
<span data-ttu-id="fa33d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa33d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="fa33d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa33d-134">Response</span></span>
<span data-ttu-id="fa33d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa33d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 906

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
      "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
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
      "profileApplicability": "androidWorkProfile"
    }
  ]
}
```





