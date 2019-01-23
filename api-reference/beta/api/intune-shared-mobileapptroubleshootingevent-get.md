---
title: Получение mobileAppTroubleshootingEvent
description: Описывает метод Get mobileAppTroubleshootingEvent Microsoft Graph API для Intune, которая поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6d151c28e909aecc1a0f20775d75813e0666df71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430569"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="f2e97-103">Получение mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f2e97-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="f2e97-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2e97-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2e97-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2e97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2e97-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2e97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e97-107">Чтение свойства и связи объекта [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f2e97-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2e97-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f2e97-108">Prerequisites</span></span>
<span data-ttu-id="f2e97-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2e97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2e97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2e97-111">Permission type</span></span>|<span data-ttu-id="f2e97-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2e97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e97-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2e97-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="f2e97-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f2e97-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="f2e97-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2e97-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f2e97-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f2e97-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="f2e97-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2e97-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f2e97-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2e97-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e97-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2e97-119">Not supported.</span></span>|
|<span data-ttu-id="f2e97-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2e97-120">Application</span></span>|<span data-ttu-id="f2e97-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2e97-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e97-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2e97-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2e97-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2e97-123">Optional query parameters</span></span>
<span data-ttu-id="f2e97-124">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2e97-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2e97-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2e97-125">Request headers</span></span>
|<span data-ttu-id="f2e97-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2e97-126">Header</span></span>|<span data-ttu-id="f2e97-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f2e97-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e97-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2e97-128">Authorization</span></span>|<span data-ttu-id="f2e97-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f2e97-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2e97-130">Accept</span><span class="sxs-lookup"><span data-stu-id="f2e97-130">Accept</span></span>|<span data-ttu-id="f2e97-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e97-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e97-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2e97-132">Request body</span></span>
<span data-ttu-id="f2e97-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2e97-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2e97-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2e97-134">Response</span></span>
<span data-ttu-id="f2e97-135">Успешно завершена, этот метод возвращает `200 OK` объект [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f2e97-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e97-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f2e97-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2e97-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2e97-137">Request</span></span>
<span data-ttu-id="f2e97-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2e97-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="f2e97-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2e97-139">Response</span></span>
<span data-ttu-id="f2e97-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f2e97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




