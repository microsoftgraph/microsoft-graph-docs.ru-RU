---
title: Удаление Мобилеапптраублешутинжевент
description: Описывает метод Delete Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c32000aea49146c7b2239d681584da61b223a4b8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537960"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="cb5f9-103">Удаление Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="cb5f9-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="cb5f9-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb5f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb5f9-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb5f9-107">Удаляет объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="cb5f9-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb5f9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb5f9-108">Prerequisites</span></span>
<span data-ttu-id="cb5f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb5f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb5f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb5f9-111">Permission type</span></span>|<span data-ttu-id="cb5f9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb5f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb5f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb5f9-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="cb5f9-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="cb5f9-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="cb5f9-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f9-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb5f9-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="cb5f9-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="cb5f9-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f9-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb5f9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb5f9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb5f9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-119">Not supported.</span></span>|
|<span data-ttu-id="cb5f9-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb5f9-120">Application</span></span>||
|<span data-ttu-id="cb5f9-121">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="cb5f9-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="cb5f9-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f9-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb5f9-123">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="cb5f9-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="cb5f9-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f9-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb5f9-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb5f9-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="cb5f9-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb5f9-126">Request headers</span></span>
|<span data-ttu-id="cb5f9-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb5f9-127">Header</span></span>|<span data-ttu-id="cb5f9-128">Значение</span><span class="sxs-lookup"><span data-stu-id="cb5f9-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb5f9-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb5f9-129">Authorization</span></span>|<span data-ttu-id="cb5f9-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb5f9-131">Accept</span><span class="sxs-lookup"><span data-stu-id="cb5f9-131">Accept</span></span>|<span data-ttu-id="cb5f9-132">application/json</span><span class="sxs-lookup"><span data-stu-id="cb5f9-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb5f9-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb5f9-133">Request body</span></span>
<span data-ttu-id="cb5f9-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb5f9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb5f9-135">Response</span></span>
<span data-ttu-id="cb5f9-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cb5f9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cb5f9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb5f9-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb5f9-138">Request</span></span>
<span data-ttu-id="cb5f9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="cb5f9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb5f9-140">Response</span></span>
<span data-ttu-id="cb5f9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb5f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










