---
title: Удаление Мобилеапптраублешутинжевент
description: Описывает метод Delete Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4bad4b91f6285f454769a47344f80aa13ce20c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022395"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="6e6d6-103">Удаление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="6e6d6-103">Delete mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="6e6d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e6d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e6d6-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e6d6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e6d6-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e6d6-108">Удаляет объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="6e6d6-108">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e6d6-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e6d6-109">Prerequisites</span></span>
<span data-ttu-id="6e6d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e6d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e6d6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e6d6-112">Permission type</span></span>|<span data-ttu-id="6e6d6-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e6d6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e6d6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e6d6-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="6e6d6-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6e6d6-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="6e6d6-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6d6-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6e6d6-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="6e6d6-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="6e6d6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6d6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6e6d6-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e6d6-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e6d6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-120">Not supported.</span></span>|
|<span data-ttu-id="6e6d6-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e6d6-121">Application</span></span>||
|<span data-ttu-id="6e6d6-122">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6e6d6-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="6e6d6-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6d6-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6e6d6-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="6e6d6-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="6e6d6-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6d6-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e6d6-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e6d6-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="6e6d6-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e6d6-127">Request headers</span></span>
|<span data-ttu-id="6e6d6-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e6d6-128">Header</span></span>|<span data-ttu-id="6e6d6-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6e6d6-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e6d6-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e6d6-130">Authorization</span></span>|<span data-ttu-id="6e6d6-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e6d6-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6e6d6-132">Accept</span></span>|<span data-ttu-id="6e6d6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6e6d6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e6d6-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e6d6-134">Request body</span></span>
<span data-ttu-id="6e6d6-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e6d6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e6d6-136">Response</span></span>
<span data-ttu-id="6e6d6-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e6d6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6e6d6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e6d6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e6d6-139">Request</span></span>
<span data-ttu-id="6e6d6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-140">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="6e6d6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e6d6-141">Response</span></span>
<span data-ttu-id="6e6d6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e6d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













