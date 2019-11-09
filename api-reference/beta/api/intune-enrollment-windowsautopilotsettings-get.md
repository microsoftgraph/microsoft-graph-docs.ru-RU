---
title: Получение windowsAutopilotSettings
description: Чтение свойств и связей объекта windowsAutopilotSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0190f216a26b3a1941f62b319f9f284fa342300f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087196"
---
# <a name="get-windowsautopilotsettings"></a><span data-ttu-id="9b942-103">Получение windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="9b942-103">Get windowsAutopilotSettings</span></span>

> <span data-ttu-id="9b942-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b942-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b942-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b942-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b942-106">Чтение свойств и связей объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="9b942-106">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b942-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b942-107">Prerequisites</span></span>
<span data-ttu-id="9b942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b942-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b942-110">Permission type</span></span>|<span data-ttu-id="9b942-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b942-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b942-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b942-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b942-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b942-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9b942-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b942-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b942-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b942-115">Not supported.</span></span>|
|<span data-ttu-id="9b942-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b942-116">Application</span></span>|<span data-ttu-id="9b942-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b942-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b942-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b942-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b942-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9b942-119">Optional query parameters</span></span>
<span data-ttu-id="9b942-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9b942-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b942-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b942-121">Request headers</span></span>
|<span data-ttu-id="9b942-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b942-122">Header</span></span>|<span data-ttu-id="9b942-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9b942-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b942-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b942-124">Authorization</span></span>|<span data-ttu-id="9b942-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b942-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b942-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9b942-126">Accept</span></span>|<span data-ttu-id="9b942-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9b942-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b942-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b942-128">Request body</span></span>
<span data-ttu-id="9b942-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b942-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b942-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b942-130">Response</span></span>
<span data-ttu-id="9b942-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b942-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b942-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9b942-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b942-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b942-133">Request</span></span>
<span data-ttu-id="9b942-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b942-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
```

### <a name="response"></a><span data-ttu-id="9b942-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b942-135">Response</span></span>
<span data-ttu-id="9b942-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 308

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
    "id": "08c16770-6770-08c1-7067-c1087067c108",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
    "syncStatus": "inProgress"
  }
}
```






