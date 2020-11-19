---
title: Получение Андроидфорворкмобилеаппконфигуратион
description: Чтение свойств и связей объекта Андроидфорворкмобилеаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9aa76adbe515898110da2dd22dff140397f6de9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253896"
---
# <a name="get-androidforworkmobileappconfiguration"></a><span data-ttu-id="b677a-103">Получение Андроидфорворкмобилеаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b677a-103">Get androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="b677a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b677a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b677a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b677a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b677a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b677a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b677a-107">Чтение свойств и связей объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b677a-107">Read properties and relationships of the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b677a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b677a-108">Prerequisites</span></span>
<span data-ttu-id="b677a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b677a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b677a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b677a-111">Permission type</span></span>|<span data-ttu-id="b677a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b677a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b677a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b677a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b677a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b677a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b677a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b677a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b677a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b677a-116">Not supported.</span></span>|
|<span data-ttu-id="b677a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b677a-117">Application</span></span>|<span data-ttu-id="b677a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b677a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b677a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b677a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b677a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b677a-120">Optional query parameters</span></span>
<span data-ttu-id="b677a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b677a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b677a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b677a-122">Request headers</span></span>
|<span data-ttu-id="b677a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b677a-123">Header</span></span>|<span data-ttu-id="b677a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b677a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b677a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b677a-125">Authorization</span></span>|<span data-ttu-id="b677a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b677a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b677a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b677a-127">Accept</span></span>|<span data-ttu-id="b677a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b677a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b677a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b677a-129">Request body</span></span>
<span data-ttu-id="b677a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b677a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b677a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b677a-131">Response</span></span>
<span data-ttu-id="b677a-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b677a-132">If successful, this method returns a `200 OK` response code and [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b677a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b677a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b677a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b677a-134">Request</span></span>
<span data-ttu-id="b677a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b677a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b677a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b677a-136">Response</span></span>
<span data-ttu-id="b677a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b677a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 846

{
  "value": {
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
}
```




