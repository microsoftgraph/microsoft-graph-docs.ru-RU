---
title: Получение Мобилеапптраублешутинжевент
description: Описывает метод Get Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 474108fc1e6345a9fb436acf877a2aa1daf9c401
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526967"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="f3811-103">Получение Мобилеапптраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="f3811-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="f3811-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3811-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3811-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3811-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3811-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3811-107">Чтение свойств и связей объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f3811-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3811-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3811-108">Prerequisites</span></span>
<span data-ttu-id="f3811-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3811-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3811-111">Permission type</span></span>|<span data-ttu-id="f3811-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3811-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3811-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3811-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="f3811-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f3811-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="f3811-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3811-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f3811-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f3811-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="f3811-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3811-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f3811-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3811-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3811-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3811-119">Not supported.</span></span>|
|<span data-ttu-id="f3811-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3811-120">Application</span></span>|<span data-ttu-id="f3811-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3811-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3811-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3811-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3811-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3811-123">Optional query parameters</span></span>
<span data-ttu-id="f3811-124">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3811-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3811-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3811-125">Request headers</span></span>
|<span data-ttu-id="f3811-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3811-126">Header</span></span>|<span data-ttu-id="f3811-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f3811-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3811-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3811-128">Authorization</span></span>|<span data-ttu-id="f3811-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3811-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3811-130">Accept</span><span class="sxs-lookup"><span data-stu-id="f3811-130">Accept</span></span>|<span data-ttu-id="f3811-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f3811-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3811-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3811-132">Request body</span></span>
<span data-ttu-id="f3811-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3811-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3811-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3811-134">Response</span></span>
<span data-ttu-id="f3811-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3811-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3811-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f3811-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3811-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3811-137">Request</span></span>
<span data-ttu-id="f3811-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3811-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="f3811-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3811-139">Response</span></span>
<span data-ttu-id="f3811-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3811-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




