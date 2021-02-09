---
title: Список windowsQualityUpdateCatalogItems
description: Список свойств и связей объектов windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d97c24f7e216145ed9862e7117cbb074d8b1fbb9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160937"
---
# <a name="list-windowsqualityupdatecatalogitems"></a><span data-ttu-id="3c476-103">Список windowsQualityUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="3c476-103">List windowsQualityUpdateCatalogItems</span></span>

<span data-ttu-id="3c476-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c476-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c476-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c476-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c476-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c476-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c476-107">Список свойств и связей объектов [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c476-107">List properties and relationships of the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c476-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c476-108">Prerequisites</span></span>
<span data-ttu-id="3c476-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c476-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c476-111">Permission type</span></span>|<span data-ttu-id="3c476-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c476-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c476-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c476-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c476-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c476-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3c476-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c476-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c476-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c476-116">Not supported.</span></span>|
|<span data-ttu-id="3c476-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c476-117">Application</span></span>|<span data-ttu-id="3c476-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c476-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c476-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c476-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="3c476-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3c476-120">Request headers</span></span>
|<span data-ttu-id="3c476-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c476-121">Header</span></span>|<span data-ttu-id="3c476-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c476-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c476-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c476-123">Authorization</span></span>|<span data-ttu-id="3c476-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c476-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c476-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c476-125">Accept</span></span>|<span data-ttu-id="3c476-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c476-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c476-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c476-127">Request body</span></span>
<span data-ttu-id="3c476-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c476-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c476-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c476-129">Response</span></span>
<span data-ttu-id="3c476-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c476-130">If successful, this method returns a `200 OK` response code and a collection of [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c476-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3c476-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c476-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c476-132">Request</span></span>
<span data-ttu-id="3c476-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c476-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="3c476-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c476-134">Response</span></span>
<span data-ttu-id="3c476-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c476-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
      "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "kbArticleId": "Kb Article Id value",
      "classification": "security",
      "isExpeditable": true
    }
  ]
}
```




