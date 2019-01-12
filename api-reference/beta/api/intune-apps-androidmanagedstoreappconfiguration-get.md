---
title: Получение androidManagedStoreAppConfiguration
description: Чтение свойства и связи объекта androidManagedStoreAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d3bff892fec6af7290d8bfe1db1623cd9a83305
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915860"
---
# <a name="get-androidmanagedstoreappconfiguration"></a><span data-ttu-id="59216-103">Получение androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="59216-103">Get androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="59216-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="59216-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59216-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59216-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59216-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59216-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59216-107">Чтение свойства и связи объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="59216-107">Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59216-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59216-108">Prerequisites</span></span>
<span data-ttu-id="59216-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59216-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59216-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59216-111">Permission type</span></span>|<span data-ttu-id="59216-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59216-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59216-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59216-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59216-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="59216-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="59216-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59216-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59216-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59216-116">Not supported.</span></span>|
|<span data-ttu-id="59216-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59216-117">Application</span></span>|<span data-ttu-id="59216-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59216-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59216-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59216-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59216-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59216-120">Optional query parameters</span></span>
<span data-ttu-id="59216-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59216-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59216-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59216-122">Request headers</span></span>
|<span data-ttu-id="59216-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59216-123">Header</span></span>|<span data-ttu-id="59216-124">Значение</span><span class="sxs-lookup"><span data-stu-id="59216-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59216-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59216-125">Authorization</span></span>|<span data-ttu-id="59216-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="59216-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59216-127">Accept</span><span class="sxs-lookup"><span data-stu-id="59216-127">Accept</span></span>|<span data-ttu-id="59216-128">application/json</span><span class="sxs-lookup"><span data-stu-id="59216-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59216-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59216-129">Request body</span></span>
<span data-ttu-id="59216-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59216-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59216-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="59216-131">Response</span></span>
<span data-ttu-id="59216-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="59216-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59216-133">Пример</span><span class="sxs-lookup"><span data-stu-id="59216-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="59216-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="59216-134">Request</span></span>
<span data-ttu-id="59216-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59216-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="59216-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="59216-136">Response</span></span>
<span data-ttu-id="59216-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59216-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 794

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
    ]
  }
}
```





