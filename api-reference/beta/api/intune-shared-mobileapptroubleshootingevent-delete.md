---
title: Удаление Мобилеапптраублешутинжевент
description: Описывает метод Delete Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af8e4c37be4a3ffd340786b706a7bc788399880f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694279"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="879a8-103">Удаление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="879a8-103">Delete mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="879a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="879a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="879a8-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="879a8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="879a8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="879a8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="879a8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="879a8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="879a8-108">Удаляет объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="879a8-108">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="879a8-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="879a8-109">Prerequisites</span></span>
<span data-ttu-id="879a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="879a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="879a8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="879a8-112">Permission type</span></span>|<span data-ttu-id="879a8-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="879a8-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="879a8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="879a8-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="879a8-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="879a8-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="879a8-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="879a8-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="879a8-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="879a8-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="879a8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="879a8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="879a8-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="879a8-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="879a8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="879a8-120">Not supported.</span></span>|
|<span data-ttu-id="879a8-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="879a8-121">Application</span></span>||
|<span data-ttu-id="879a8-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="879a8-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="879a8-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="879a8-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="879a8-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="879a8-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="879a8-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="879a8-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="879a8-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="879a8-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="879a8-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="879a8-127">Request headers</span></span>
|<span data-ttu-id="879a8-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="879a8-128">Header</span></span>|<span data-ttu-id="879a8-129">Значение</span><span class="sxs-lookup"><span data-stu-id="879a8-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="879a8-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="879a8-130">Authorization</span></span>|<span data-ttu-id="879a8-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="879a8-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="879a8-132">Accept</span><span class="sxs-lookup"><span data-stu-id="879a8-132">Accept</span></span>|<span data-ttu-id="879a8-133">application/json</span><span class="sxs-lookup"><span data-stu-id="879a8-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="879a8-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="879a8-134">Request body</span></span>
<span data-ttu-id="879a8-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="879a8-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="879a8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="879a8-136">Response</span></span>
<span data-ttu-id="879a8-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="879a8-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="879a8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="879a8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="879a8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="879a8-139">Request</span></span>
<span data-ttu-id="879a8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="879a8-140">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="879a8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="879a8-141">Response</span></span>
<span data-ttu-id="879a8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="879a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












