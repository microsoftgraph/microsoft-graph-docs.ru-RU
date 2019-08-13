---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07c019135c8777d63e0990ca6bd742f75a4d88d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336728"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="dfac0-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dfac0-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="dfac0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfac0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfac0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfac0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfac0-106">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dfac0-106">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfac0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dfac0-107">Prerequisites</span></span>
<span data-ttu-id="dfac0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfac0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfac0-110">Permission type</span></span>|<span data-ttu-id="dfac0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfac0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfac0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfac0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfac0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfac0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dfac0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfac0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfac0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfac0-115">Not supported.</span></span>|
|<span data-ttu-id="dfac0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfac0-116">Application</span></span>|<span data-ttu-id="dfac0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfac0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfac0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfac0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="dfac0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfac0-119">Request headers</span></span>
|<span data-ttu-id="dfac0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfac0-120">Header</span></span>|<span data-ttu-id="dfac0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dfac0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfac0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfac0-122">Authorization</span></span>|<span data-ttu-id="dfac0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfac0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfac0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dfac0-124">Accept</span></span>|<span data-ttu-id="dfac0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfac0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfac0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfac0-126">Request body</span></span>
<span data-ttu-id="dfac0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfac0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfac0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfac0-128">Response</span></span>
<span data-ttu-id="dfac0-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfac0-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfac0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dfac0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfac0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfac0-131">Request</span></span>
<span data-ttu-id="dfac0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfac0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="dfac0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfac0-133">Response</span></span>
<span data-ttu-id="dfac0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfac0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```






