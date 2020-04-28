---
title: Получение Девицехеалсскриптассигнмент
description: Чтение свойств и связей объекта Девицехеалсскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 003c286b3f068d05e25de7e3b10ba210613075cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426209"
---
# <a name="get-devicehealthscriptassignment"></a><span data-ttu-id="fef05-103">Получение Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="fef05-103">Get deviceHealthScriptAssignment</span></span>

<span data-ttu-id="fef05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fef05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fef05-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fef05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef05-107">Чтение свойств и связей объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fef05-107">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fef05-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fef05-108">Prerequisites</span></span>
<span data-ttu-id="fef05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fef05-111">Permission type</span></span>|<span data-ttu-id="fef05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fef05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fef05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fef05-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fef05-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fef05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fef05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef05-116">Not supported.</span></span>|
|<span data-ttu-id="fef05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fef05-117">Application</span></span>|<span data-ttu-id="fef05-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fef05-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fef05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fef05-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fef05-120">Optional query parameters</span></span>
<span data-ttu-id="fef05-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fef05-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fef05-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fef05-122">Request headers</span></span>
|<span data-ttu-id="fef05-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fef05-123">Header</span></span>|<span data-ttu-id="fef05-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fef05-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fef05-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fef05-125">Authorization</span></span>|<span data-ttu-id="fef05-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef05-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fef05-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fef05-127">Accept</span></span>|<span data-ttu-id="fef05-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fef05-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef05-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fef05-129">Request body</span></span>
<span data-ttu-id="fef05-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fef05-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fef05-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fef05-131">Response</span></span>
<span data-ttu-id="fef05-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fef05-132">If successful, this method returns a `200 OK` response code and [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef05-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fef05-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef05-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fef05-134">Request</span></span>
<span data-ttu-id="fef05-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fef05-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="fef05-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef05-136">Response</span></span>
<span data-ttu-id="fef05-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fef05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
    "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "runRemediationScript": true,
    "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
    }
  }
}
```



