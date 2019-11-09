---
title: Перечисление объектов mobileApp
description: Список свойств и связей объектов mobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b8e58adf460d57908848b85f8c9fa0d36acd46b
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085768"
---
# <a name="list-mobileapps"></a><span data-ttu-id="1cdb2-103">Перечисление объектов mobileApp</span><span class="sxs-lookup"><span data-stu-id="1cdb2-103">List mobileApps</span></span>

> <span data-ttu-id="1cdb2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cdb2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cdb2-106">Список свойств и связей объектов [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cdb2-106">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cdb2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1cdb2-107">Prerequisites</span></span>
<span data-ttu-id="1cdb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cdb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cdb2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cdb2-110">Permission type</span></span>|<span data-ttu-id="1cdb2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cdb2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cdb2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cdb2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1cdb2-113">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="1cdb2-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="1cdb2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cdb2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="1cdb2-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="1cdb2-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1cdb2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cdb2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1cdb2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cdb2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cdb2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-118">Not supported.</span></span>|
|<span data-ttu-id="1cdb2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cdb2-119">Application</span></span>||
| <span data-ttu-id="1cdb2-120">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="1cdb2-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="1cdb2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cdb2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="1cdb2-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="1cdb2-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1cdb2-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cdb2-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cdb2-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cdb2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1cdb2-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1cdb2-125">Request headers</span></span>
|<span data-ttu-id="1cdb2-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cdb2-126">Header</span></span>|<span data-ttu-id="1cdb2-127">Значение</span><span class="sxs-lookup"><span data-stu-id="1cdb2-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cdb2-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cdb2-128">Authorization</span></span>|<span data-ttu-id="1cdb2-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cdb2-130">Accept</span><span class="sxs-lookup"><span data-stu-id="1cdb2-130">Accept</span></span>|<span data-ttu-id="1cdb2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1cdb2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cdb2-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cdb2-132">Request body</span></span>
<span data-ttu-id="1cdb2-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cdb2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cdb2-134">Response</span></span>
<span data-ttu-id="1cdb2-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileApp](../resources/intune-shared-mobileapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-135">If successful, this method returns a `200 OK` response code and a collection of [mobileApp](../resources/intune-shared-mobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cdb2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1cdb2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cdb2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cdb2-137">Request</span></span>
<span data-ttu-id="1cdb2-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="1cdb2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cdb2-139">Response</span></span>
<span data-ttu-id="1cdb2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cdb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









