---
title: Получение Андроидманажедстореаппконфигуратион
description: Чтение свойств и связей объекта Андроидманажедстореаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5682401f620473bb59588b2e44e055d5c9ee2b97
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39922042"
---
# <a name="get-androidmanagedstoreappconfiguration"></a><span data-ttu-id="65aa2-103">Получение Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="65aa2-103">Get androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="65aa2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65aa2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65aa2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65aa2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65aa2-106">Чтение свойств и связей объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="65aa2-106">Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65aa2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65aa2-107">Prerequisites</span></span>
<span data-ttu-id="65aa2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65aa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65aa2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65aa2-110">Permission type</span></span>|<span data-ttu-id="65aa2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65aa2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65aa2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65aa2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65aa2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65aa2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="65aa2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65aa2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65aa2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65aa2-115">Not supported.</span></span>|
|<span data-ttu-id="65aa2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65aa2-116">Application</span></span>|<span data-ttu-id="65aa2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65aa2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65aa2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65aa2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65aa2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65aa2-119">Optional query parameters</span></span>
<span data-ttu-id="65aa2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="65aa2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65aa2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65aa2-121">Request headers</span></span>
|<span data-ttu-id="65aa2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65aa2-122">Header</span></span>|<span data-ttu-id="65aa2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="65aa2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65aa2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65aa2-124">Authorization</span></span>|<span data-ttu-id="65aa2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65aa2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65aa2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="65aa2-126">Accept</span></span>|<span data-ttu-id="65aa2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="65aa2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65aa2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65aa2-128">Request body</span></span>
<span data-ttu-id="65aa2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65aa2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65aa2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="65aa2-130">Response</span></span>
<span data-ttu-id="65aa2-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65aa2-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65aa2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="65aa2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="65aa2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="65aa2-133">Request</span></span>
<span data-ttu-id="65aa2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65aa2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="65aa2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="65aa2-135">Response</span></span>
<span data-ttu-id="65aa2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65aa2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
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
    "appSupportsOemConfig": true
  }
}
```





