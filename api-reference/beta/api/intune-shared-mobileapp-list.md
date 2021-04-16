---
title: Перечисление объектов mobileApp
description: Список свойств и связей объектов mobileApp.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec574543622428f86aca4cdaa2f3136102748417
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865875"
---
# <a name="list-mobileapps"></a><span data-ttu-id="a6b08-103">Перечисление объектов mobileApp</span><span class="sxs-lookup"><span data-stu-id="a6b08-103">List mobileApps</span></span>

<span data-ttu-id="a6b08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6b08-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6b08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6b08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6b08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6b08-107">Список свойств и связей объектов [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6b08-107">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6b08-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a6b08-108">Prerequisites</span></span>
<span data-ttu-id="a6b08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6b08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6b08-111">Permission type</span></span>|<span data-ttu-id="a6b08-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6b08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6b08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6b08-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a6b08-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="a6b08-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="a6b08-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6b08-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="a6b08-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a6b08-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a6b08-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6b08-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6b08-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6b08-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6b08-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6b08-119">Not supported.</span></span>|
|<span data-ttu-id="a6b08-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a6b08-120">Application</span></span>||
| <span data-ttu-id="a6b08-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="a6b08-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="a6b08-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6b08-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="a6b08-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a6b08-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a6b08-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6b08-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6b08-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6b08-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a6b08-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a6b08-126">Request headers</span></span>
|<span data-ttu-id="a6b08-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6b08-127">Header</span></span>|<span data-ttu-id="a6b08-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a6b08-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6b08-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6b08-129">Authorization</span></span>|<span data-ttu-id="a6b08-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6b08-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6b08-131">Accept</span><span class="sxs-lookup"><span data-stu-id="a6b08-131">Accept</span></span>|<span data-ttu-id="a6b08-132">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b08-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6b08-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6b08-133">Request body</span></span>
<span data-ttu-id="a6b08-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6b08-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6b08-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6b08-135">Response</span></span>
<span data-ttu-id="a6b08-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileApp](../resources/intune-shared-mobileapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6b08-136">If successful, this method returns a `200 OK` response code and a collection of [mobileApp](../resources/intune-shared-mobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b08-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a6b08-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6b08-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6b08-138">Request</span></span>
<span data-ttu-id="a6b08-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6b08-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a6b08-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6b08-140">Response</span></span>
<span data-ttu-id="a6b08-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6b08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







