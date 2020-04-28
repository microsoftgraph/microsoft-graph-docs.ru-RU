---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c8b9532aa4d950149b155cefd5e35da7ddf720a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43404621"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="85e94-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="85e94-103">List mobileAppAssignments</span></span>

<span data-ttu-id="85e94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85e94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85e94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85e94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85e94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e94-107">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="85e94-107">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85e94-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85e94-108">Prerequisites</span></span>
<span data-ttu-id="85e94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85e94-111">Permission type</span></span>|<span data-ttu-id="85e94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85e94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85e94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85e94-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="85e94-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="85e94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85e94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85e94-116">Not supported.</span></span>|
|<span data-ttu-id="85e94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85e94-117">Application</span></span>|<span data-ttu-id="85e94-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="85e94-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85e94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="85e94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85e94-120">Request headers</span></span>
|<span data-ttu-id="85e94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85e94-121">Header</span></span>|<span data-ttu-id="85e94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85e94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e94-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85e94-123">Authorization</span></span>|<span data-ttu-id="85e94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85e94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85e94-125">Accept</span></span>|<span data-ttu-id="85e94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85e94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85e94-127">Request body</span></span>
<span data-ttu-id="85e94-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85e94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85e94-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="85e94-129">Response</span></span>
<span data-ttu-id="85e94-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85e94-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e94-131">Пример</span><span class="sxs-lookup"><span data-stu-id="85e94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="85e94-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="85e94-132">Request</span></span>
<span data-ttu-id="85e94-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85e94-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="85e94-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="85e94-134">Response</span></span>
<span data-ttu-id="85e94-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85e94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

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
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



