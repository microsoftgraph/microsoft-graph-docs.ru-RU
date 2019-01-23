---
title: Список mobileAppTroubleshootingEvents
description: Описание метода mobileAppTroubleshootingEvent списка Microsoft Graph API для Intune, которая поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79f89fd755b52bc0d9a3a1a1d0e0c6dc91853e76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430734"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="88de9-103">Список mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="88de9-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="88de9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88de9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88de9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88de9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88de9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88de9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88de9-107">Свойства списка и связей объектов [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="88de9-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88de9-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="88de9-108">Prerequisites</span></span>
<span data-ttu-id="88de9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88de9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88de9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88de9-111">Permission type</span></span>|<span data-ttu-id="88de9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88de9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88de9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88de9-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="88de9-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="88de9-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="88de9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88de9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="88de9-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="88de9-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="88de9-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88de9-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="88de9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88de9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88de9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88de9-119">Not supported.</span></span>|
|<span data-ttu-id="88de9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88de9-120">Application</span></span>|<span data-ttu-id="88de9-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88de9-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88de9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88de9-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="88de9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88de9-123">Request headers</span></span>
|<span data-ttu-id="88de9-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88de9-124">Header</span></span>|<span data-ttu-id="88de9-125">Значение</span><span class="sxs-lookup"><span data-stu-id="88de9-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88de9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88de9-126">Authorization</span></span>|<span data-ttu-id="88de9-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="88de9-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88de9-128">Accept</span><span class="sxs-lookup"><span data-stu-id="88de9-128">Accept</span></span>|<span data-ttu-id="88de9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="88de9-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88de9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88de9-130">Request body</span></span>
<span data-ttu-id="88de9-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88de9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88de9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="88de9-132">Response</span></span>
<span data-ttu-id="88de9-133">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="88de9-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88de9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="88de9-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="88de9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="88de9-135">Request</span></span>
<span data-ttu-id="88de9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88de9-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="88de9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="88de9-137">Response</span></span>
<span data-ttu-id="88de9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="88de9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




