---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 007abe193ffa77fb22b72cf40288f5d56ab31c4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761337"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="0d795-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="0d795-103">List mobileAppContents</span></span>

> <span data-ttu-id="0d795-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d795-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d795-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d795-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d795-106">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="0d795-106">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d795-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d795-107">Prerequisites</span></span>
<span data-ttu-id="0d795-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d795-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d795-110">Permission type</span></span>|<span data-ttu-id="0d795-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d795-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d795-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d795-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d795-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d795-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0d795-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d795-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d795-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d795-115">Not supported.</span></span>|
|<span data-ttu-id="0d795-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d795-116">Application</span></span>|<span data-ttu-id="0d795-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d795-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d795-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d795-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="0d795-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d795-119">Request headers</span></span>
|<span data-ttu-id="0d795-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d795-120">Header</span></span>|<span data-ttu-id="0d795-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d795-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d795-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d795-122">Authorization</span></span>|<span data-ttu-id="0d795-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d795-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d795-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d795-124">Accept</span></span>|<span data-ttu-id="0d795-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d795-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d795-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d795-126">Request body</span></span>
<span data-ttu-id="0d795-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d795-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d795-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d795-128">Response</span></span>
<span data-ttu-id="0d795-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d795-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d795-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0d795-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d795-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d795-131">Request</span></span>
<span data-ttu-id="0d795-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d795-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="0d795-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d795-133">Response</span></span>
<span data-ttu-id="0d795-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d795-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```




