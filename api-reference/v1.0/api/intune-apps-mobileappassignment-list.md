---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbc50a8bdf27aad35a9a846a8b9e13775ebb3376
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255677"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="0e78b-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="0e78b-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="0e78b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e78b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e78b-105">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0e78b-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e78b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e78b-106">Prerequisites</span></span>
<span data-ttu-id="0e78b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e78b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e78b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e78b-109">Permission type</span></span>|<span data-ttu-id="0e78b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e78b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e78b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e78b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e78b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e78b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0e78b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e78b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e78b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e78b-114">Not supported.</span></span>|
|<span data-ttu-id="0e78b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e78b-115">Application</span></span>|<span data-ttu-id="0e78b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e78b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e78b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e78b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0e78b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e78b-118">Request headers</span></span>
|<span data-ttu-id="0e78b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e78b-119">Header</span></span>|<span data-ttu-id="0e78b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0e78b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e78b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e78b-121">Authorization</span></span>|<span data-ttu-id="0e78b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e78b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e78b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0e78b-123">Accept</span></span>|<span data-ttu-id="0e78b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e78b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e78b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e78b-125">Request body</span></span>
<span data-ttu-id="0e78b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e78b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e78b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e78b-127">Response</span></span>
<span data-ttu-id="0e78b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e78b-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e78b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0e78b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e78b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e78b-130">Request</span></span>
<span data-ttu-id="0e78b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e78b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="0e78b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e78b-132">Response</span></span>
<span data-ttu-id="0e78b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e78b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



