---
title: Список windowsUpdateCatalogItems
description: Список свойств и связей объектов WindowsUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f4be6933c7218fdf4c51e2172aa7b487a7718b0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865630"
---
# <a name="list-windowsupdatecatalogitems"></a><span data-ttu-id="9c1b9-103">Список windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="9c1b9-103">List windowsUpdateCatalogItems</span></span>

<span data-ttu-id="9c1b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c1b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c1b9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c1b9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c1b9-107">Список свойств и связей [объектов WindowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="9c1b9-107">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c1b9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c1b9-108">Prerequisites</span></span>
<span data-ttu-id="9c1b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c1b9-111">Permission type</span></span>|<span data-ttu-id="9c1b9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c1b9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c1b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1b9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c1b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c1b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-116">Not supported.</span></span>|
|<span data-ttu-id="9c1b9-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9c1b9-117">Application</span></span>|<span data-ttu-id="9c1b9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1b9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c1b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="9c1b9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9c1b9-120">Request headers</span></span>
|<span data-ttu-id="9c1b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c1b9-121">Header</span></span>|<span data-ttu-id="9c1b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c1b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1b9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c1b9-123">Authorization</span></span>|<span data-ttu-id="9c1b9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c1b9-125">Accept</span></span>|<span data-ttu-id="9c1b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c1b9-127">Request body</span></span>
<span data-ttu-id="9c1b9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c1b9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c1b9-129">Response</span></span>
<span data-ttu-id="9c1b9-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1b9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9c1b9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c1b9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c1b9-132">Request</span></span>
<span data-ttu-id="9c1b9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="9c1b9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c1b9-134">Response</span></span>
<span data-ttu-id="9c1b9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c1b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
      "id": "e887145d-145d-e887-5d14-87e85d1487e8",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
    }
  ]
}
```




