---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbaf9b6e6ed656079019904e7037d3e9ca8ea701
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754079"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="4cc99-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4cc99-103">List mobileAppContents</span></span>

<span data-ttu-id="4cc99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cc99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cc99-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cc99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cc99-106">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4cc99-106">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cc99-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4cc99-107">Prerequisites</span></span>
<span data-ttu-id="4cc99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cc99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cc99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cc99-110">Permission type</span></span>|<span data-ttu-id="4cc99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cc99-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cc99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cc99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cc99-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cc99-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4cc99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cc99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cc99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cc99-115">Not supported.</span></span>|
|<span data-ttu-id="4cc99-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4cc99-116">Application</span></span>|<span data-ttu-id="4cc99-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cc99-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cc99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cc99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="4cc99-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4cc99-119">Request headers</span></span>
|<span data-ttu-id="4cc99-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cc99-120">Header</span></span>|<span data-ttu-id="4cc99-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4cc99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cc99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cc99-122">Authorization</span></span>|<span data-ttu-id="4cc99-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cc99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cc99-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4cc99-124">Accept</span></span>|<span data-ttu-id="4cc99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cc99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cc99-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cc99-126">Request body</span></span>
<span data-ttu-id="4cc99-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cc99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cc99-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cc99-128">Response</span></span>
<span data-ttu-id="4cc99-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cc99-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cc99-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4cc99-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cc99-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cc99-131">Request</span></span>
<span data-ttu-id="4cc99-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cc99-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="4cc99-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cc99-133">Response</span></span>
<span data-ttu-id="4cc99-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cc99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




