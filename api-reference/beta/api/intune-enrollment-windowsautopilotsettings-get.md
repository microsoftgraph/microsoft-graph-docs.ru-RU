---
title: Получение windowsAutopilotSettings
description: Чтение свойства и связи объекта windowsAutopilotSettings.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17c8c9aae7294beb7716aba696a6cce77022fccb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854371"
---
# <a name="get-windowsautopilotsettings"></a><span data-ttu-id="2a789-103">Получение windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2a789-103">Get windowsAutopilotSettings</span></span>

> <span data-ttu-id="2a789-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2a789-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a789-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a789-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a789-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2a789-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a789-107">Чтение свойства и связи объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="2a789-107">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a789-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a789-108">Prerequisites</span></span>
<span data-ttu-id="2a789-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a789-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a789-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a789-111">Permission type</span></span>|<span data-ttu-id="2a789-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a789-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a789-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a789-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a789-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a789-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2a789-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a789-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a789-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a789-116">Not supported.</span></span>|
|<span data-ttu-id="2a789-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a789-117">Application</span></span>|<span data-ttu-id="2a789-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a789-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a789-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a789-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a789-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a789-120">Optional query parameters</span></span>
<span data-ttu-id="2a789-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a789-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2a789-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a789-122">Request headers</span></span>
|<span data-ttu-id="2a789-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a789-123">Header</span></span>|<span data-ttu-id="2a789-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2a789-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a789-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a789-125">Authorization</span></span>|<span data-ttu-id="2a789-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2a789-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a789-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2a789-127">Accept</span></span>|<span data-ttu-id="2a789-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2a789-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a789-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a789-129">Request body</span></span>
<span data-ttu-id="2a789-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a789-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a789-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a789-131">Response</span></span>
<span data-ttu-id="2a789-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2a789-132">If successful, this method returns a `200 OK` response code and [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a789-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2a789-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a789-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a789-134">Request</span></span>
<span data-ttu-id="2a789-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a789-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
```

### <a name="response"></a><span data-ttu-id="2a789-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a789-136">Response</span></span>
<span data-ttu-id="2a789-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2a789-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





