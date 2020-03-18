---
title: Список Мобилеапптраублешутинжевентс
description: Описывает метод List Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fdb3b3acfb4d378db05a05b25eff1d321efe40cf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800734"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="d6b96-103">Список Мобилеапптраублешутинжевентс</span><span class="sxs-lookup"><span data-stu-id="d6b96-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="d6b96-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6b96-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d6b96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6b96-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6b96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6b96-107">Список свойств и связей объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b96-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6b96-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6b96-108">Prerequisites</span></span>
<span data-ttu-id="d6b96-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b96-111">Permission type</span></span>|<span data-ttu-id="d6b96-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6b96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6b96-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="d6b96-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d6b96-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="d6b96-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b96-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d6b96-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d6b96-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="d6b96-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b96-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d6b96-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6b96-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b96-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b96-119">Not supported.</span></span>|
|<span data-ttu-id="d6b96-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6b96-120">Application</span></span>||
|<span data-ttu-id="d6b96-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d6b96-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="d6b96-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b96-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d6b96-123">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d6b96-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="d6b96-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b96-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6b96-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6b96-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d6b96-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6b96-126">Request headers</span></span>
|<span data-ttu-id="d6b96-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6b96-127">Header</span></span>|<span data-ttu-id="d6b96-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d6b96-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6b96-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b96-129">Authorization</span></span>|<span data-ttu-id="d6b96-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6b96-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6b96-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d6b96-131">Accept</span></span>|<span data-ttu-id="d6b96-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b96-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b96-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6b96-133">Request body</span></span>
<span data-ttu-id="d6b96-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6b96-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6b96-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6b96-135">Response</span></span>
<span data-ttu-id="d6b96-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6b96-136">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b96-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d6b96-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6b96-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6b96-138">Request</span></span>
<span data-ttu-id="d6b96-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6b96-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="d6b96-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b96-140">Response</span></span>
<span data-ttu-id="d6b96-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6b96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











