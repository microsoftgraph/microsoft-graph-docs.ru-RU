---
title: Список windowsAppXs
description: Свойства списка и связей объектов windowsAppX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 86547dff2a7f7c8cf6a3040f4003a1f5d834ac81
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417310"
---
# <a name="list-windowsappxs"></a><span data-ttu-id="5d069-103">Список windowsAppXs</span><span class="sxs-lookup"><span data-stu-id="5d069-103">List windowsAppXs</span></span>

> <span data-ttu-id="5d069-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d069-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d069-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d069-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d069-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d069-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d069-107">Свойства списка и связей объектов [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="5d069-107">List properties and relationships of the [windowsAppX](../resources/intune-apps-windowsappx.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d069-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5d069-108">Prerequisites</span></span>
<span data-ttu-id="5d069-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d069-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5d069-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d069-111">Permission type</span></span>|<span data-ttu-id="5d069-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d069-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d069-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d069-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d069-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d069-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5d069-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d069-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d069-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d069-116">Not supported.</span></span>|
|<span data-ttu-id="5d069-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d069-117">Application</span></span>|<span data-ttu-id="5d069-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d069-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d069-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d069-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5d069-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d069-120">Request headers</span></span>
|<span data-ttu-id="5d069-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d069-121">Header</span></span>|<span data-ttu-id="5d069-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d069-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d069-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d069-123">Authorization</span></span>|<span data-ttu-id="5d069-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5d069-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d069-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d069-125">Accept</span></span>|<span data-ttu-id="5d069-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d069-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d069-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d069-127">Request body</span></span>
<span data-ttu-id="5d069-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d069-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d069-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d069-129">Response</span></span>
<span data-ttu-id="5d069-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsAppX](../resources/intune-apps-windowsappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5d069-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAppX](../resources/intune-apps-windowsappx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d069-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5d069-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d069-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d069-132">Request</span></span>
<span data-ttu-id="5d069-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d069-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5d069-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d069-134">Response</span></span>
<span data-ttu-id="5d069-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5d069-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1717

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAppX",
      "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "applicableArchitectures": "x86",
      "identityName": "Identity Name value",
      "identityPublisherHash": "Identity Publisher Hash value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "isBundle": true,
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      },
      "identityVersion": "Identity Version value"
    }
  ]
}
```




