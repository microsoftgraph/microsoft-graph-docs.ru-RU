---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d0ce557104532275664cb9d9afec40da2a56784
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167601"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="e6536-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e6536-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="e6536-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6536-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6536-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6536-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6536-106">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="e6536-106">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6536-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e6536-107">Prerequisites</span></span>
<span data-ttu-id="e6536-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6536-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6536-110">Permission type</span></span>|<span data-ttu-id="e6536-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6536-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6536-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6536-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6536-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6536-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e6536-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6536-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6536-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6536-115">Not supported.</span></span>|
|<span data-ttu-id="e6536-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6536-116">Application</span></span>|<span data-ttu-id="e6536-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6536-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6536-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6536-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="e6536-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6536-119">Request headers</span></span>
|<span data-ttu-id="e6536-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6536-120">Header</span></span>|<span data-ttu-id="e6536-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6536-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6536-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6536-122">Authorization</span></span>|<span data-ttu-id="e6536-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6536-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6536-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6536-124">Accept</span></span>|<span data-ttu-id="e6536-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6536-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6536-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6536-126">Request body</span></span>
<span data-ttu-id="e6536-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6536-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6536-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6536-128">Response</span></span>
<span data-ttu-id="e6536-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6536-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6536-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e6536-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6536-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6536-131">Request</span></span>
<span data-ttu-id="e6536-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6536-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="e6536-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6536-133">Response</span></span>
<span data-ttu-id="e6536-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContentFile",
      "azureStorageUri": "Azure Storage Uri value",
      "isCommitted": true,
      "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "name": "Name value",
      "size": 4,
      "sizeEncrypted": 13,
      "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
      "manifest": "bWFuaWZlc3Q=",
      "uploadState": "transientError",
      "isFrameworkFile": true,
      "isDependency": true
    }
  ]
}
```




