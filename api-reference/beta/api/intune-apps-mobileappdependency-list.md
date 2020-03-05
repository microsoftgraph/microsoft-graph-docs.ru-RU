---
title: Список МобилеаппдепенденЦиес
description: Список свойств и связей объектов Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80ea3bc802d72ebc92fa2ee1f3999c3c6a3c2877
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450715"
---
# <a name="list-mobileappdependencies"></a><span data-ttu-id="0a987-103">Список МобилеаппдепенденЦиес</span><span class="sxs-lookup"><span data-stu-id="0a987-103">List mobileAppDependencies</span></span>

<span data-ttu-id="0a987-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0a987-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a987-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a987-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a987-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a987-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a987-107">Список свойств и связей объектов [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="0a987-107">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a987-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a987-108">Prerequisites</span></span>
<span data-ttu-id="0a987-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a987-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a987-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a987-111">Permission type</span></span>|<span data-ttu-id="0a987-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a987-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a987-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a987-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a987-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a987-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a987-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a987-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a987-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a987-116">Not supported.</span></span>|
|<span data-ttu-id="0a987-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a987-117">Application</span></span>|<span data-ttu-id="0a987-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a987-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a987-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a987-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="0a987-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a987-120">Request headers</span></span>
|<span data-ttu-id="0a987-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a987-121">Header</span></span>|<span data-ttu-id="0a987-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a987-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a987-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a987-123">Authorization</span></span>|<span data-ttu-id="0a987-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a987-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a987-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a987-125">Accept</span></span>|<span data-ttu-id="0a987-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a987-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a987-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a987-127">Request body</span></span>
<span data-ttu-id="0a987-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a987-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a987-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a987-129">Response</span></span>
<span data-ttu-id="0a987-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a987-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a987-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0a987-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a987-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a987-132">Request</span></span>
<span data-ttu-id="0a987-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a987-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="0a987-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a987-134">Response</span></span>
<span data-ttu-id="0a987-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a987-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppDependency",
      "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "dependencyType": "autoInstall",
      "dependentAppCount": 1
    }
  ]
}
```





