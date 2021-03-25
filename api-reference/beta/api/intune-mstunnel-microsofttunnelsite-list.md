---
title: Список microsoftTunnelSites
description: Список свойств и связей объектов microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8efcfe80d49055a92666abf18f7a8fa282e06032
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152939"
---
# <a name="list-microsofttunnelsites"></a><span data-ttu-id="84dfd-103">Список microsoftTunnelSites</span><span class="sxs-lookup"><span data-stu-id="84dfd-103">List microsoftTunnelSites</span></span>

<span data-ttu-id="84dfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84dfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84dfd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84dfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84dfd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84dfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84dfd-107">Список свойств и связей объектов [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)</span><span class="sxs-lookup"><span data-stu-id="84dfd-107">List properties and relationships of the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84dfd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84dfd-108">Prerequisites</span></span>
<span data-ttu-id="84dfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84dfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84dfd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84dfd-111">Permission type</span></span>|<span data-ttu-id="84dfd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84dfd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84dfd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84dfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84dfd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84dfd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84dfd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84dfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84dfd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84dfd-116">Not supported.</span></span>|
|<span data-ttu-id="84dfd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="84dfd-117">Application</span></span>|<span data-ttu-id="84dfd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84dfd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84dfd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84dfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a><span data-ttu-id="84dfd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84dfd-120">Request headers</span></span>
|<span data-ttu-id="84dfd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84dfd-121">Header</span></span>|<span data-ttu-id="84dfd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84dfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84dfd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84dfd-123">Authorization</span></span>|<span data-ttu-id="84dfd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84dfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84dfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84dfd-125">Accept</span></span>|<span data-ttu-id="84dfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84dfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84dfd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84dfd-127">Request body</span></span>
<span data-ttu-id="84dfd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84dfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84dfd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="84dfd-129">Response</span></span>
<span data-ttu-id="84dfd-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84dfd-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84dfd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="84dfd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="84dfd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="84dfd-132">Request</span></span>
<span data-ttu-id="84dfd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84dfd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
```

### <a name="response"></a><span data-ttu-id="84dfd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="84dfd-134">Response</span></span>
<span data-ttu-id="84dfd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84dfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 360

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelSite",
      "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
      "displayName": "Display Name value",
      "description": "Description value",
      "publicAddress": "Public Address value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




