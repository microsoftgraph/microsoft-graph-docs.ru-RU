---
title: Перечисление объектов mobileAppCategory
description: Список свойств и связей объектов mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30fbde724596506696b6194490b50d5de06db06c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935267"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="9b283-103">Перечисление объектов mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="9b283-103">List mobileAppCategories</span></span>

> <span data-ttu-id="9b283-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b283-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b283-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b283-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b283-106">Список свойств и связей объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="9b283-106">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b283-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9b283-107">Prerequisites</span></span>
<span data-ttu-id="9b283-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b283-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b283-110">Permission type</span></span>|<span data-ttu-id="9b283-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b283-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b283-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b283-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b283-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b283-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9b283-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b283-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b283-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b283-115">Not supported.</span></span>|
|<span data-ttu-id="9b283-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b283-116">Application</span></span>|<span data-ttu-id="9b283-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b283-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b283-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b283-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="9b283-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b283-119">Request headers</span></span>
|<span data-ttu-id="9b283-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b283-120">Header</span></span>|<span data-ttu-id="9b283-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9b283-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b283-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b283-122">Authorization</span></span>|<span data-ttu-id="9b283-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b283-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b283-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9b283-124">Accept</span></span>|<span data-ttu-id="9b283-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b283-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b283-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b283-126">Request body</span></span>
<span data-ttu-id="9b283-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b283-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b283-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b283-128">Response</span></span>
<span data-ttu-id="9b283-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b283-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b283-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9b283-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b283-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b283-131">Request</span></span>
<span data-ttu-id="9b283-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b283-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="9b283-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b283-133">Response</span></span>
<span data-ttu-id="9b283-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b283-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




