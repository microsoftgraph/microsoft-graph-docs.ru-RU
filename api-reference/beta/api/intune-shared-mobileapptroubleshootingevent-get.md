---
title: Get mobileAppTroubleshootingEvent
description: Описывает метод Get mobileAppTroubleshootingEvent API Microsoft Graph для Intune, который поддерживает несколько процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e74e1e979ab501f45a9a3e93fe9a64bdb30320d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863740"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="19b33-103">Get mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="19b33-103">Get mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="19b33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19b33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19b33-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="19b33-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19b33-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b33-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19b33-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19b33-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19b33-108">Чтение свойств и связей объекта [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="19b33-108">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19b33-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19b33-109">Prerequisites</span></span>
<span data-ttu-id="19b33-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b33-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19b33-112">Permission type</span></span>|<span data-ttu-id="19b33-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19b33-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19b33-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19b33-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="19b33-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="19b33-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="19b33-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b33-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="19b33-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="19b33-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="19b33-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b33-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="19b33-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19b33-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19b33-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b33-120">Not supported.</span></span>|
|<span data-ttu-id="19b33-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="19b33-121">Application</span></span>||
|<span data-ttu-id="19b33-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="19b33-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="19b33-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b33-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="19b33-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="19b33-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="19b33-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b33-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b33-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19b33-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19b33-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19b33-127">Optional query parameters</span></span>
<span data-ttu-id="19b33-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19b33-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19b33-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19b33-129">Request headers</span></span>
|<span data-ttu-id="19b33-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19b33-130">Header</span></span>|<span data-ttu-id="19b33-131">Значение</span><span class="sxs-lookup"><span data-stu-id="19b33-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19b33-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19b33-132">Authorization</span></span>|<span data-ttu-id="19b33-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19b33-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19b33-134">Accept</span><span class="sxs-lookup"><span data-stu-id="19b33-134">Accept</span></span>|<span data-ttu-id="19b33-135">application/json</span><span class="sxs-lookup"><span data-stu-id="19b33-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b33-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19b33-136">Request body</span></span>
<span data-ttu-id="19b33-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19b33-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19b33-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b33-138">Response</span></span>
<span data-ttu-id="19b33-139">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="19b33-139">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b33-140">Пример</span><span class="sxs-lookup"><span data-stu-id="19b33-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="19b33-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="19b33-141">Request</span></span>
<span data-ttu-id="19b33-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19b33-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="19b33-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b33-143">Response</span></span>
<span data-ttu-id="19b33-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19b33-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477"
  }
}
```











