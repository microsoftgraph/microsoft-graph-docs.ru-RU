---
title: Список androidManagedStoreAppConfigurations
description: Свойства списка и связей объектов androidManagedStoreAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75fec07bd23b4b8a3412743ad99b1cb0370e0fd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424758"
---
# <a name="list-androidmanagedstoreappconfigurations"></a><span data-ttu-id="56211-103">Список androidManagedStoreAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="56211-103">List androidManagedStoreAppConfigurations</span></span>

> <span data-ttu-id="56211-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56211-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56211-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56211-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56211-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56211-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56211-107">Свойства списка и связей объектов [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="56211-107">List properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56211-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="56211-108">Prerequisites</span></span>
<span data-ttu-id="56211-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="56211-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="56211-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56211-111">Permission type</span></span>|<span data-ttu-id="56211-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56211-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56211-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56211-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56211-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="56211-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="56211-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56211-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56211-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56211-116">Not supported.</span></span>|
|<span data-ttu-id="56211-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56211-117">Application</span></span>|<span data-ttu-id="56211-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56211-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56211-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56211-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56211-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56211-120">Request headers</span></span>
|<span data-ttu-id="56211-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56211-121">Header</span></span>|<span data-ttu-id="56211-122">Значение</span><span class="sxs-lookup"><span data-stu-id="56211-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56211-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56211-123">Authorization</span></span>|<span data-ttu-id="56211-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="56211-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56211-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56211-125">Accept</span></span>|<span data-ttu-id="56211-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56211-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56211-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56211-127">Request body</span></span>
<span data-ttu-id="56211-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56211-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56211-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="56211-129">Response</span></span>
<span data-ttu-id="56211-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56211-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56211-131">Пример</span><span class="sxs-lookup"><span data-stu-id="56211-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="56211-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="56211-132">Request</span></span>
<span data-ttu-id="56211-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56211-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="56211-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="56211-134">Response</span></span>
<span data-ttu-id="56211-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56211-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

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
      ]
    }
  ]
}
```




