---
title: Перечисление объектов mobileAppCategory
description: Список свойств и связей объектов mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bca59d6be158dc2f21d70765dea8d443dc0138b9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248919"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="89934-103">Перечисление объектов mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="89934-103">List mobileAppCategories</span></span>

<span data-ttu-id="89934-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89934-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89934-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89934-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89934-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89934-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89934-107">Список свойств и связей объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="89934-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89934-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89934-108">Prerequisites</span></span>
<span data-ttu-id="89934-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89934-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89934-111">Permission type</span></span>|<span data-ttu-id="89934-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89934-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89934-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89934-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89934-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="89934-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="89934-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89934-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89934-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89934-116">Not supported.</span></span>|
|<span data-ttu-id="89934-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="89934-117">Application</span></span>|<span data-ttu-id="89934-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="89934-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89934-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89934-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="89934-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89934-120">Request headers</span></span>
|<span data-ttu-id="89934-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89934-121">Header</span></span>|<span data-ttu-id="89934-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89934-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89934-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89934-123">Authorization</span></span>|<span data-ttu-id="89934-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89934-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89934-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89934-125">Accept</span></span>|<span data-ttu-id="89934-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89934-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89934-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89934-127">Request body</span></span>
<span data-ttu-id="89934-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89934-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89934-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="89934-129">Response</span></span>
<span data-ttu-id="89934-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89934-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89934-131">Пример</span><span class="sxs-lookup"><span data-stu-id="89934-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="89934-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89934-132">Request</span></span>
<span data-ttu-id="89934-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89934-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="89934-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="89934-134">Response</span></span>
<span data-ttu-id="89934-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89934-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




