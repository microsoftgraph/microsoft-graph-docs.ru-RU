---
title: Get mobileApp
description: Чтение свойств и связей объекта mobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba82569d8a5f709e03ea14e4079212b0b26ad142
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261925"
---
# <a name="get-mobileapp"></a><span data-ttu-id="d88ce-103">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="d88ce-103">Get mobileApp</span></span>

<span data-ttu-id="d88ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d88ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d88ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d88ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d88ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d88ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88ce-107">Чтение свойств и связей объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d88ce-107">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d88ce-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d88ce-108">Prerequisites</span></span>
<span data-ttu-id="d88ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d88ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d88ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d88ce-111">Permission type</span></span>|<span data-ttu-id="d88ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d88ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d88ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d88ce-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d88ce-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="d88ce-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d88ce-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88ce-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="d88ce-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d88ce-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d88ce-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88ce-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d88ce-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d88ce-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d88ce-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d88ce-119">Not supported.</span></span>|
|<span data-ttu-id="d88ce-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="d88ce-120">Application</span></span>||
| <span data-ttu-id="d88ce-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="d88ce-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d88ce-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88ce-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="d88ce-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d88ce-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d88ce-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88ce-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d88ce-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d88ce-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d88ce-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d88ce-126">Optional query parameters</span></span>
<span data-ttu-id="d88ce-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d88ce-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d88ce-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d88ce-128">Request headers</span></span>
|<span data-ttu-id="d88ce-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d88ce-129">Header</span></span>|<span data-ttu-id="d88ce-130">Значение</span><span class="sxs-lookup"><span data-stu-id="d88ce-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d88ce-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d88ce-131">Authorization</span></span>|<span data-ttu-id="d88ce-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d88ce-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d88ce-133">Accept</span><span class="sxs-lookup"><span data-stu-id="d88ce-133">Accept</span></span>|<span data-ttu-id="d88ce-134">application/json</span><span class="sxs-lookup"><span data-stu-id="d88ce-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d88ce-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d88ce-135">Request body</span></span>
<span data-ttu-id="d88ce-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d88ce-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d88ce-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d88ce-137">Response</span></span>
<span data-ttu-id="d88ce-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileApp](../resources/intune-shared-mobileapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d88ce-138">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-shared-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d88ce-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d88ce-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d88ce-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d88ce-140">Request</span></span>
<span data-ttu-id="d88ce-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d88ce-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d88ce-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d88ce-142">Response</span></span>
<span data-ttu-id="d88ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d88ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 949

{
  "value": {
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
}
```







