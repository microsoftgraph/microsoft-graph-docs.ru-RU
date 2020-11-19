---
title: Список Конфигманажерколлектионс
description: Список свойств и связей объектов Конфигманажерколлектион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 165ed79f911fb0ef8505d75029e28cdf1003eb93
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337127"
---
# <a name="list-configmanagercollections"></a><span data-ttu-id="49eab-103">Список Конфигманажерколлектионс</span><span class="sxs-lookup"><span data-stu-id="49eab-103">List configManagerCollections</span></span>

<span data-ttu-id="49eab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49eab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49eab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49eab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49eab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49eab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49eab-107">Список свойств и связей объектов [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) .</span><span class="sxs-lookup"><span data-stu-id="49eab-107">List properties and relationships of the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49eab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49eab-108">Prerequisites</span></span>
<span data-ttu-id="49eab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49eab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49eab-111">Permission type</span></span>|<span data-ttu-id="49eab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49eab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49eab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49eab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49eab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="49eab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="49eab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49eab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49eab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49eab-116">Not supported.</span></span>|
|<span data-ttu-id="49eab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49eab-117">Application</span></span>|<span data-ttu-id="49eab-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="49eab-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49eab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49eab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="49eab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49eab-120">Request headers</span></span>
|<span data-ttu-id="49eab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49eab-121">Header</span></span>|<span data-ttu-id="49eab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49eab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49eab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49eab-123">Authorization</span></span>|<span data-ttu-id="49eab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49eab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49eab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49eab-125">Accept</span></span>|<span data-ttu-id="49eab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49eab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49eab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49eab-127">Request body</span></span>
<span data-ttu-id="49eab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49eab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49eab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="49eab-129">Response</span></span>
<span data-ttu-id="49eab-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49eab-130">If successful, this method returns a `200 OK` response code and a collection of [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49eab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="49eab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="49eab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="49eab-132">Request</span></span>
<span data-ttu-id="49eab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49eab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
```

### <a name="response"></a><span data-ttu-id="49eab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="49eab-134">Response</span></span>
<span data-ttu-id="49eab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49eab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.configManagerCollection",
      "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
      "displayName": "Display Name value",
      "collectionIdentifier": "Collection Identifier value",
      "hierarchyName": "Hierarchy Name value",
      "hierarchyIdentifier": "Hierarchy Identifier value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




