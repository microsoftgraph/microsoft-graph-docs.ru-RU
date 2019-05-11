---
title: Получение Мобилеапптраублешутинжевент
description: Описывает метод Get Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 2237edd34ab4a6e22032db997e45ed98bee570f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898684"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="2f86e-103">Получение Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="2f86e-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="2f86e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f86e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f86e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f86e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f86e-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f86e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f86e-107">Чтение свойств и связей объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="2f86e-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f86e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f86e-108">Prerequisites</span></span>
<span data-ttu-id="2f86e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f86e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f86e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f86e-111">Permission type</span></span>|<span data-ttu-id="2f86e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f86e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f86e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f86e-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="2f86e-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2f86e-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="2f86e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f86e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2f86e-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="2f86e-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="2f86e-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f86e-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2f86e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f86e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f86e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f86e-119">Not supported.</span></span>|
|<span data-ttu-id="2f86e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f86e-120">Application</span></span>|<span data-ttu-id="2f86e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f86e-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f86e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f86e-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f86e-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f86e-123">Optional query parameters</span></span>
<span data-ttu-id="2f86e-124">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f86e-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f86e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f86e-125">Request headers</span></span>
|<span data-ttu-id="2f86e-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f86e-126">Header</span></span>|<span data-ttu-id="2f86e-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2f86e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f86e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f86e-128">Authorization</span></span>|<span data-ttu-id="2f86e-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f86e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f86e-130">Accept</span><span class="sxs-lookup"><span data-stu-id="2f86e-130">Accept</span></span>|<span data-ttu-id="2f86e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2f86e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f86e-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f86e-132">Request body</span></span>
<span data-ttu-id="2f86e-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f86e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f86e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f86e-134">Response</span></span>
<span data-ttu-id="2f86e-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f86e-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f86e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2f86e-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f86e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f86e-137">Request</span></span>
<span data-ttu-id="2f86e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f86e-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="2f86e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f86e-139">Response</span></span>
<span data-ttu-id="2f86e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f86e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




