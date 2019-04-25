---
title: Список Мобилеапптраублешутинжевентс
description: Описывает метод List Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d34d37324e61e967b01b46e2a1ba842688862281
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526988"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="c5d38-103">Список Мобилеапптраублешутинжевентс</span><span class="sxs-lookup"><span data-stu-id="c5d38-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="c5d38-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5d38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5d38-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5d38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5d38-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5d38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5d38-107">Список свойств и связей объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d38-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5d38-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5d38-108">Prerequisites</span></span>
<span data-ttu-id="c5d38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5d38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5d38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5d38-111">Permission type</span></span>|<span data-ttu-id="c5d38-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5d38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5d38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5d38-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c5d38-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c5d38-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c5d38-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5d38-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c5d38-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c5d38-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c5d38-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5d38-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c5d38-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5d38-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5d38-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5d38-119">Not supported.</span></span>|
|<span data-ttu-id="c5d38-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5d38-120">Application</span></span>|<span data-ttu-id="c5d38-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5d38-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5d38-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5d38-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="c5d38-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5d38-123">Request headers</span></span>
|<span data-ttu-id="c5d38-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5d38-124">Header</span></span>|<span data-ttu-id="c5d38-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c5d38-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5d38-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5d38-126">Authorization</span></span>|<span data-ttu-id="c5d38-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5d38-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5d38-128">Accept</span><span class="sxs-lookup"><span data-stu-id="c5d38-128">Accept</span></span>|<span data-ttu-id="c5d38-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d38-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d38-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5d38-130">Request body</span></span>
<span data-ttu-id="c5d38-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5d38-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5d38-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5d38-132">Response</span></span>
<span data-ttu-id="c5d38-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5d38-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d38-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c5d38-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5d38-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5d38-135">Request</span></span>
<span data-ttu-id="c5d38-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5d38-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="c5d38-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5d38-137">Response</span></span>
<span data-ttu-id="c5d38-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5d38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




