---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9be3b4ed71929bc1aa09205d5b95a89a247b5dfe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990245"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="f415e-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="f415e-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="f415e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f415e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f415e-105">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f415e-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f415e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f415e-106">Prerequisites</span></span>
<span data-ttu-id="f415e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f415e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f415e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f415e-109">Permission type</span></span>|<span data-ttu-id="f415e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f415e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f415e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f415e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f415e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f415e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f415e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f415e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f415e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f415e-114">Not supported.</span></span>|
|<span data-ttu-id="f415e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f415e-115">Application</span></span>|<span data-ttu-id="f415e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f415e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f415e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f415e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f415e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f415e-118">Request headers</span></span>
|<span data-ttu-id="f415e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f415e-119">Header</span></span>|<span data-ttu-id="f415e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f415e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f415e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f415e-121">Authorization</span></span>|<span data-ttu-id="f415e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f415e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f415e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f415e-123">Accept</span></span>|<span data-ttu-id="f415e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f415e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f415e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f415e-125">Request body</span></span>
<span data-ttu-id="f415e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f415e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f415e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f415e-127">Response</span></span>
<span data-ttu-id="f415e-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f415e-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f415e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f415e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f415e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f415e-130">Request</span></span>
<span data-ttu-id="f415e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f415e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="f415e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f415e-132">Response</span></span>
<span data-ttu-id="f415e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f415e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



