---
title: Удаление Мобилеапптраублешутинжевент
description: Описывает метод Delete Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76bd23a97e6fda06ae6dc012dbd98150ea3b6f4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458240"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="ce937-103">Удаление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="ce937-103">Delete mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="ce937-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce937-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce937-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce937-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce937-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce937-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce937-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce937-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce937-108">Удаляет объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ce937-108">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce937-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce937-109">Prerequisites</span></span>
<span data-ttu-id="ce937-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce937-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce937-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce937-112">Permission type</span></span>|<span data-ttu-id="ce937-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce937-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce937-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce937-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ce937-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ce937-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ce937-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce937-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ce937-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="ce937-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ce937-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce937-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ce937-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce937-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce937-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce937-120">Not supported.</span></span>|
|<span data-ttu-id="ce937-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce937-121">Application</span></span>||
|<span data-ttu-id="ce937-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ce937-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ce937-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce937-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ce937-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="ce937-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ce937-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce937-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce937-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce937-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="ce937-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce937-127">Request headers</span></span>
|<span data-ttu-id="ce937-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce937-128">Header</span></span>|<span data-ttu-id="ce937-129">Значение</span><span class="sxs-lookup"><span data-stu-id="ce937-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce937-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce937-130">Authorization</span></span>|<span data-ttu-id="ce937-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce937-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce937-132">Accept</span><span class="sxs-lookup"><span data-stu-id="ce937-132">Accept</span></span>|<span data-ttu-id="ce937-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ce937-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce937-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce937-134">Request body</span></span>
<span data-ttu-id="ce937-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce937-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce937-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce937-136">Response</span></span>
<span data-ttu-id="ce937-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce937-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ce937-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ce937-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce937-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce937-139">Request</span></span>
<span data-ttu-id="ce937-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce937-140">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ce937-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce937-141">Response</span></span>
<span data-ttu-id="ce937-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce937-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












