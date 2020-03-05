---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8539240df4e92a75ac21aa2cb97c389295236ae6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450757"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="7ec77-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7ec77-103">List mobileAppContents</span></span>

<span data-ttu-id="7ec77-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7ec77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ec77-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ec77-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ec77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ec77-107">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7ec77-107">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ec77-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ec77-108">Prerequisites</span></span>
<span data-ttu-id="7ec77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ec77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ec77-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ec77-111">Permission type</span></span>|<span data-ttu-id="7ec77-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ec77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ec77-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ec77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ec77-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ec77-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7ec77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ec77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ec77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec77-116">Not supported.</span></span>|
|<span data-ttu-id="7ec77-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ec77-117">Application</span></span>|<span data-ttu-id="7ec77-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ec77-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ec77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ec77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="7ec77-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ec77-120">Request headers</span></span>
|<span data-ttu-id="7ec77-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ec77-121">Header</span></span>|<span data-ttu-id="7ec77-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7ec77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ec77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ec77-123">Authorization</span></span>|<span data-ttu-id="7ec77-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ec77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ec77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ec77-125">Accept</span></span>|<span data-ttu-id="7ec77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ec77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ec77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ec77-127">Request body</span></span>
<span data-ttu-id="7ec77-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ec77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ec77-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ec77-129">Response</span></span>
<span data-ttu-id="7ec77-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ec77-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ec77-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7ec77-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ec77-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ec77-132">Request</span></span>
<span data-ttu-id="7ec77-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ec77-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="7ec77-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ec77-134">Response</span></span>
<span data-ttu-id="7ec77-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ec77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





