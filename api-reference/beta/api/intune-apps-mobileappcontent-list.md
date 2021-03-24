---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9bce10c6c418989b28d976cf166ee90fc8d719f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143285"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="ce4db-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ce4db-103">List mobileAppContents</span></span>

<span data-ttu-id="ce4db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce4db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce4db-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce4db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce4db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce4db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce4db-107">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ce4db-107">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce4db-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ce4db-108">Prerequisites</span></span>
<span data-ttu-id="ce4db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce4db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce4db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce4db-111">Permission type</span></span>|<span data-ttu-id="ce4db-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce4db-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce4db-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce4db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce4db-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4db-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce4db-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce4db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce4db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce4db-116">Not supported.</span></span>|
|<span data-ttu-id="ce4db-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce4db-117">Application</span></span>|<span data-ttu-id="ce4db-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4db-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce4db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce4db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="ce4db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce4db-120">Request headers</span></span>
|<span data-ttu-id="ce4db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce4db-121">Header</span></span>|<span data-ttu-id="ce4db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce4db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce4db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce4db-123">Authorization</span></span>|<span data-ttu-id="ce4db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce4db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce4db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce4db-125">Accept</span></span>|<span data-ttu-id="ce4db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce4db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce4db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce4db-127">Request body</span></span>
<span data-ttu-id="ce4db-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce4db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce4db-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce4db-129">Response</span></span>
<span data-ttu-id="ce4db-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce4db-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce4db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ce4db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce4db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce4db-132">Request</span></span>
<span data-ttu-id="ce4db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce4db-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="ce4db-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce4db-134">Response</span></span>
<span data-ttu-id="ce4db-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce4db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




