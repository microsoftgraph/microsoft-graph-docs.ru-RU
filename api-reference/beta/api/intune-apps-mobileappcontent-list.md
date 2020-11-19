---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aeebe566e2b29dfe1880e7512fcf6d278944a943
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248877"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="9e3d1-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9e3d1-103">List mobileAppContents</span></span>

<span data-ttu-id="9e3d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e3d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e3d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e3d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e3d1-107">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="9e3d1-107">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e3d1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9e3d1-108">Prerequisites</span></span>
<span data-ttu-id="9e3d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e3d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e3d1-111">Permission type</span></span>|<span data-ttu-id="9e3d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e3d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e3d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e3d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e3d1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e3d1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9e3d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e3d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e3d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-116">Not supported.</span></span>|
|<span data-ttu-id="9e3d1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e3d1-117">Application</span></span>|<span data-ttu-id="9e3d1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e3d1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e3d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e3d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="9e3d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9e3d1-120">Request headers</span></span>
|<span data-ttu-id="9e3d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e3d1-121">Header</span></span>|<span data-ttu-id="9e3d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9e3d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e3d1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e3d1-123">Authorization</span></span>|<span data-ttu-id="9e3d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e3d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e3d1-125">Accept</span></span>|<span data-ttu-id="9e3d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e3d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e3d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e3d1-127">Request body</span></span>
<span data-ttu-id="9e3d1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e3d1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e3d1-129">Response</span></span>
<span data-ttu-id="9e3d1-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e3d1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e3d1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e3d1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e3d1-132">Request</span></span>
<span data-ttu-id="9e3d1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="9e3d1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e3d1-134">Response</span></span>
<span data-ttu-id="9e3d1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e3d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




