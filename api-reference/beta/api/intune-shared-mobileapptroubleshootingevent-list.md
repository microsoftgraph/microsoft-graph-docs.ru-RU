---
title: Список mobileAppTroubleshootingEvents
description: Описывает метод List mobileAppTroubleshootingEvent API Microsoft Graph для Intune, который поддерживает несколько процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 537ddbb686950346c699e1462f6992991a318620
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863707"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="85bbc-103">Список mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="85bbc-103">List mobileAppTroubleshootingEvents</span></span>

<span data-ttu-id="85bbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85bbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85bbc-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="85bbc-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85bbc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85bbc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85bbc-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85bbc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85bbc-108">Список свойств и связей объектов [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="85bbc-108">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85bbc-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85bbc-109">Prerequisites</span></span>
<span data-ttu-id="85bbc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85bbc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85bbc-112">Permission type</span></span>|<span data-ttu-id="85bbc-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85bbc-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85bbc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85bbc-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="85bbc-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="85bbc-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="85bbc-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="85bbc-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="85bbc-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="85bbc-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="85bbc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="85bbc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="85bbc-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85bbc-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85bbc-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85bbc-120">Not supported.</span></span>|
|<span data-ttu-id="85bbc-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="85bbc-121">Application</span></span>||
|<span data-ttu-id="85bbc-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="85bbc-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="85bbc-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="85bbc-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="85bbc-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="85bbc-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="85bbc-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="85bbc-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85bbc-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85bbc-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="85bbc-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85bbc-127">Request headers</span></span>
|<span data-ttu-id="85bbc-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85bbc-128">Header</span></span>|<span data-ttu-id="85bbc-129">Значение</span><span class="sxs-lookup"><span data-stu-id="85bbc-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85bbc-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85bbc-130">Authorization</span></span>|<span data-ttu-id="85bbc-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85bbc-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85bbc-132">Accept</span><span class="sxs-lookup"><span data-stu-id="85bbc-132">Accept</span></span>|<span data-ttu-id="85bbc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="85bbc-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85bbc-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85bbc-134">Request body</span></span>
<span data-ttu-id="85bbc-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85bbc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85bbc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="85bbc-136">Response</span></span>
<span data-ttu-id="85bbc-137">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85bbc-137">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85bbc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="85bbc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="85bbc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="85bbc-139">Request</span></span>
<span data-ttu-id="85bbc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85bbc-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="85bbc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="85bbc-141">Response</span></span>
<span data-ttu-id="85bbc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85bbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```











