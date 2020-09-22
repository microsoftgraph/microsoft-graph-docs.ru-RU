---
title: Перечисление объектов mobileApp
description: Список свойств и связей объектов mobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4694c8ee7929688fbee52feffb44bae24722d091
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095879"
---
# <a name="list-mobileapps"></a><span data-ttu-id="f2d6d-103">Перечисление объектов mobileApp</span><span class="sxs-lookup"><span data-stu-id="f2d6d-103">List mobileApps</span></span>

<span data-ttu-id="f2d6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2d6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2d6d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2d6d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2d6d-107">Список свойств и связей объектов [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2d6d-107">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2d6d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f2d6d-108">Prerequisites</span></span>
<span data-ttu-id="f2d6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2d6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2d6d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2d6d-111">Permission type</span></span>|<span data-ttu-id="f2d6d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2d6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2d6d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2d6d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f2d6d-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="f2d6d-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="f2d6d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2d6d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="f2d6d-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f2d6d-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f2d6d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2d6d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2d6d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2d6d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2d6d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-119">Not supported.</span></span>|
|<span data-ttu-id="f2d6d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2d6d-120">Application</span></span>||
| <span data-ttu-id="f2d6d-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="f2d6d-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="f2d6d-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2d6d-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="f2d6d-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f2d6d-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f2d6d-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2d6d-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2d6d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2d6d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f2d6d-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2d6d-126">Request headers</span></span>
|<span data-ttu-id="f2d6d-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2d6d-127">Header</span></span>|<span data-ttu-id="f2d6d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="f2d6d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2d6d-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2d6d-129">Authorization</span></span>|<span data-ttu-id="f2d6d-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2d6d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="f2d6d-131">Accept</span></span>|<span data-ttu-id="f2d6d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f2d6d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2d6d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2d6d-133">Request body</span></span>
<span data-ttu-id="f2d6d-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2d6d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2d6d-135">Response</span></span>
<span data-ttu-id="f2d6d-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileApp](../resources/intune-shared-mobileapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-136">If successful, this method returns a `200 OK` response code and a collection of [mobileApp](../resources/intune-shared-mobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2d6d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f2d6d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2d6d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2d6d-138">Request</span></span>
<span data-ttu-id="f2d6d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f2d6d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2d6d-140">Response</span></span>
<span data-ttu-id="f2d6d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      "dependentAppCount": 1
    }
  ]
}
```









