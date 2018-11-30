---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
ms.openlocfilehash: 8a4cbd101678e9a712a30ffeaf3c0196d807fa1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025682"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="0377a-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="0377a-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="0377a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0377a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0377a-105">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0377a-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0377a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0377a-106">Prerequisites</span></span>
<span data-ttu-id="0377a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0377a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0377a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0377a-109">Permission type</span></span>|<span data-ttu-id="0377a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0377a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0377a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0377a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0377a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0377a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0377a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0377a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0377a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0377a-114">Not supported.</span></span>|
|<span data-ttu-id="0377a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0377a-115">Application</span></span>|<span data-ttu-id="0377a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0377a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0377a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0377a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0377a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0377a-118">Request headers</span></span>
|<span data-ttu-id="0377a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0377a-119">Header</span></span>|<span data-ttu-id="0377a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0377a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0377a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0377a-121">Authorization</span></span>|<span data-ttu-id="0377a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0377a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0377a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0377a-123">Accept</span></span>|<span data-ttu-id="0377a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0377a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0377a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0377a-125">Request body</span></span>
<span data-ttu-id="0377a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0377a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0377a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0377a-127">Response</span></span>
<span data-ttu-id="0377a-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0377a-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0377a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0377a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0377a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0377a-130">Request</span></span>
<span data-ttu-id="0377a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0377a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="0377a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0377a-132">Response</span></span>
<span data-ttu-id="0377a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0377a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



