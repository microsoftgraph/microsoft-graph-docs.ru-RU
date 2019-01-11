---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0c412c05a0a9e0755aba7b933379b7eda3e26a50
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870178"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="253ab-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="253ab-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="253ab-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="253ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="253ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="253ab-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="253ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="253ab-107">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="253ab-107">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="253ab-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="253ab-108">Prerequisites</span></span>
<span data-ttu-id="253ab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="253ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="253ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="253ab-111">Permission type</span></span>|<span data-ttu-id="253ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="253ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="253ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="253ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="253ab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="253ab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="253ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="253ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="253ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253ab-116">Not supported.</span></span>|
|<span data-ttu-id="253ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="253ab-117">Application</span></span>|<span data-ttu-id="253ab-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="253ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="253ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="253ab-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="253ab-120">Request headers</span></span>
|<span data-ttu-id="253ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="253ab-121">Header</span></span>|<span data-ttu-id="253ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="253ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="253ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="253ab-123">Authorization</span></span>|<span data-ttu-id="253ab-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="253ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="253ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="253ab-125">Accept</span></span>|<span data-ttu-id="253ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="253ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="253ab-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="253ab-127">Request body</span></span>
<span data-ttu-id="253ab-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="253ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="253ab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="253ab-129">Response</span></span>
<span data-ttu-id="253ab-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="253ab-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="253ab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="253ab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="253ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="253ab-132">Request</span></span>
<span data-ttu-id="253ab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="253ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="253ab-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="253ab-134">Response</span></span>
<span data-ttu-id="253ab-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="253ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





