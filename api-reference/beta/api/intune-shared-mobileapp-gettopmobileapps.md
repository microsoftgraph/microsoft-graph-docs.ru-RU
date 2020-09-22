---
title: Функция getTopMobileApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc5697df9862ce1b17361ba3ec6b5b9c0a573463
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053848"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="468fd-103">Функция getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="468fd-103">getTopMobileApps function</span></span>

<span data-ttu-id="468fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="468fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="468fd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="468fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="468fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="468fd-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="468fd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="468fd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="468fd-108">Prerequisites</span></span>
<span data-ttu-id="468fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="468fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="468fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="468fd-111">Permission type</span></span>|<span data-ttu-id="468fd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="468fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="468fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="468fd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="468fd-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="468fd-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="468fd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="468fd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="468fd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="468fd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="468fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468fd-117">Not supported.</span></span>|
|<span data-ttu-id="468fd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="468fd-118">Application</span></span>||
| <span data-ttu-id="468fd-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="468fd-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="468fd-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="468fd-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="468fd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="468fd-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="468fd-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="468fd-122">Request headers</span></span>
|<span data-ttu-id="468fd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="468fd-123">Header</span></span>|<span data-ttu-id="468fd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="468fd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="468fd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="468fd-125">Authorization</span></span>|<span data-ttu-id="468fd-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="468fd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="468fd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="468fd-127">Accept</span></span>|<span data-ttu-id="468fd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="468fd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="468fd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="468fd-129">Request body</span></span>
<span data-ttu-id="468fd-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="468fd-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="468fd-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="468fd-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="468fd-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="468fd-132">Property</span></span>|<span data-ttu-id="468fd-133">Тип</span><span class="sxs-lookup"><span data-stu-id="468fd-133">Type</span></span>|<span data-ttu-id="468fd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="468fd-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="468fd-135">status</span><span class="sxs-lookup"><span data-stu-id="468fd-135">status</span></span>|<span data-ttu-id="468fd-136">String</span><span class="sxs-lookup"><span data-stu-id="468fd-136">String</span></span>|<span data-ttu-id="468fd-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="468fd-137">Not yet documented</span></span>|
|<span data-ttu-id="468fd-138">count</span><span class="sxs-lookup"><span data-stu-id="468fd-138">count</span></span>|<span data-ttu-id="468fd-139">Int64</span><span class="sxs-lookup"><span data-stu-id="468fd-139">Int64</span></span>|<span data-ttu-id="468fd-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="468fd-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="468fd-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="468fd-141">Response</span></span>
<span data-ttu-id="468fd-142">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [mobileApp](../resources/intune-shared-mobileapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="468fd-142">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="468fd-143">Пример</span><span class="sxs-lookup"><span data-stu-id="468fd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="468fd-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="468fd-144">Request</span></span>
<span data-ttu-id="468fd-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="468fd-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="468fd-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="468fd-146">Response</span></span>
<span data-ttu-id="468fd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="468fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









