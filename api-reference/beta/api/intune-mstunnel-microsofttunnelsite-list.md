---
title: Список Микрософттуннелситес
description: Список свойств и связей объектов Микрософттуннелсите.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edefc1f378a3f80eecfd10131712b39fc3a3e186
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301945"
---
# <a name="list-microsofttunnelsites"></a><span data-ttu-id="6e582-103">Список Микрософттуннелситес</span><span class="sxs-lookup"><span data-stu-id="6e582-103">List microsoftTunnelSites</span></span>

<span data-ttu-id="6e582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e582-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e582-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e582-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e582-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e582-107">Список свойств и связей объектов [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) .</span><span class="sxs-lookup"><span data-stu-id="6e582-107">List properties and relationships of the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e582-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e582-108">Prerequisites</span></span>
<span data-ttu-id="6e582-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e582-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e582-111">Permission type</span></span>|<span data-ttu-id="6e582-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e582-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e582-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e582-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e582-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e582-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6e582-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e582-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e582-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e582-116">Not supported.</span></span>|
|<span data-ttu-id="6e582-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e582-117">Application</span></span>|<span data-ttu-id="6e582-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e582-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e582-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e582-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a><span data-ttu-id="6e582-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e582-120">Request headers</span></span>
|<span data-ttu-id="6e582-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e582-121">Header</span></span>|<span data-ttu-id="6e582-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e582-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e582-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e582-123">Authorization</span></span>|<span data-ttu-id="6e582-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e582-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e582-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e582-125">Accept</span></span>|<span data-ttu-id="6e582-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e582-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e582-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e582-127">Request body</span></span>
<span data-ttu-id="6e582-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e582-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e582-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e582-129">Response</span></span>
<span data-ttu-id="6e582-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e582-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e582-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6e582-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e582-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e582-132">Request</span></span>
<span data-ttu-id="6e582-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e582-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
```

### <a name="response"></a><span data-ttu-id="6e582-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e582-134">Response</span></span>
<span data-ttu-id="6e582-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e582-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




