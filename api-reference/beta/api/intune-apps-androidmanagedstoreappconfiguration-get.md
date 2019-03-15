---
title: Получение Андроидманажедстореаппконфигуратион
description: Чтение свойств и связей объекта Андроидманажедстореаппконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b884077e602d02b6302c8ba36a7339e82e761d53
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571601"
---
# <a name="get-androidmanagedstoreappconfiguration"></a><span data-ttu-id="fcdee-103">Получение Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="fcdee-103">Get androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="fcdee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcdee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcdee-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcdee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcdee-106">Чтение свойств и связей объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fcdee-106">Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcdee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fcdee-107">Prerequisites</span></span>
<span data-ttu-id="fcdee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcdee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fcdee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcdee-110">Permission type</span></span>|<span data-ttu-id="fcdee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcdee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcdee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcdee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fcdee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcdee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fcdee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcdee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcdee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcdee-115">Not supported.</span></span>|
|<span data-ttu-id="fcdee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcdee-116">Application</span></span>|<span data-ttu-id="fcdee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcdee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcdee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcdee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcdee-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcdee-119">Optional query parameters</span></span>
<span data-ttu-id="fcdee-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcdee-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcdee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcdee-121">Request headers</span></span>
|<span data-ttu-id="fcdee-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcdee-122">Header</span></span>|<span data-ttu-id="fcdee-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fcdee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcdee-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcdee-124">Authorization</span></span>|<span data-ttu-id="fcdee-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcdee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcdee-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fcdee-126">Accept</span></span>|<span data-ttu-id="fcdee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fcdee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcdee-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcdee-128">Request body</span></span>
<span data-ttu-id="fcdee-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcdee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcdee-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcdee-130">Response</span></span>
<span data-ttu-id="fcdee-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcdee-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcdee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fcdee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcdee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcdee-133">Request</span></span>
<span data-ttu-id="fcdee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcdee-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fcdee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcdee-135">Response</span></span>
<span data-ttu-id="fcdee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcdee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




