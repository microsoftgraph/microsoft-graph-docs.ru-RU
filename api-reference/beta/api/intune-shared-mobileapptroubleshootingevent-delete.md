---
title: Удаление mobileAppTroubleshootingEvent
description: Описывает метод Delete mobileAppTroubleshootingEvent API Microsoft Graph для Intune, который поддерживает несколько процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b44012db5d7a22aa2d1ec10371e26a48731c7df1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863761"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="c066e-103">Удаление mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c066e-103">Delete mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="c066e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c066e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c066e-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="c066e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c066e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c066e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c066e-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c066e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c066e-108">Удаляет [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c066e-108">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c066e-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c066e-109">Prerequisites</span></span>
<span data-ttu-id="c066e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c066e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c066e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c066e-112">Permission type</span></span>|<span data-ttu-id="c066e-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c066e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c066e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c066e-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c066e-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c066e-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c066e-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c066e-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c066e-117">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c066e-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c066e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c066e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c066e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c066e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c066e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c066e-120">Not supported.</span></span>|
|<span data-ttu-id="c066e-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c066e-121">Application</span></span>||
|<span data-ttu-id="c066e-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c066e-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c066e-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c066e-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c066e-124">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c066e-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c066e-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c066e-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c066e-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c066e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c066e-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c066e-127">Request headers</span></span>
|<span data-ttu-id="c066e-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c066e-128">Header</span></span>|<span data-ttu-id="c066e-129">Значение</span><span class="sxs-lookup"><span data-stu-id="c066e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c066e-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c066e-130">Authorization</span></span>|<span data-ttu-id="c066e-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c066e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c066e-132">Accept</span><span class="sxs-lookup"><span data-stu-id="c066e-132">Accept</span></span>|<span data-ttu-id="c066e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c066e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c066e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c066e-134">Request body</span></span>
<span data-ttu-id="c066e-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c066e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c066e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c066e-136">Response</span></span>
<span data-ttu-id="c066e-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c066e-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c066e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c066e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c066e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c066e-139">Request</span></span>
<span data-ttu-id="c066e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c066e-140">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="c066e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c066e-141">Response</span></span>
<span data-ttu-id="c066e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c066e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











