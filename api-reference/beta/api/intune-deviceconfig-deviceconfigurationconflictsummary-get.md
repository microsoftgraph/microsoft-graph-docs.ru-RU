---
title: Получение deviceConfigurationConflictSummary
description: Чтение свойства и связи объекта deviceConfigurationConflictSummary.
ms.openlocfilehash: 85af2e1ffcacc5d3944680afdc6a80b4e72b1213
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080043"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="67842-103">Получение deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="67842-103">Get deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="67842-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67842-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67842-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67842-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67842-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67842-107">Чтение свойства и связи объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="67842-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67842-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67842-108">Prerequisites</span></span>
<span data-ttu-id="67842-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67842-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67842-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67842-111">Permission type</span></span>|<span data-ttu-id="67842-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67842-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67842-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67842-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67842-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="67842-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="67842-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67842-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67842-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67842-116">Not supported.</span></span>|
|<span data-ttu-id="67842-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67842-117">Application</span></span>|<span data-ttu-id="67842-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67842-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67842-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67842-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67842-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67842-120">Optional query parameters</span></span>
<span data-ttu-id="67842-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67842-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="67842-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67842-122">Request headers</span></span>
|<span data-ttu-id="67842-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67842-123">Header</span></span>|<span data-ttu-id="67842-124">Значение</span><span class="sxs-lookup"><span data-stu-id="67842-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67842-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="67842-125">Authorization</span></span>|<span data-ttu-id="67842-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="67842-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67842-127">Accept</span><span class="sxs-lookup"><span data-stu-id="67842-127">Accept</span></span>|<span data-ttu-id="67842-128">application/json</span><span class="sxs-lookup"><span data-stu-id="67842-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67842-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67842-129">Request body</span></span>
<span data-ttu-id="67842-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67842-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67842-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="67842-131">Response</span></span>
<span data-ttu-id="67842-132">Успешно завершена, этот метод возвращает `200 OK` объект [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="67842-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67842-133">Пример</span><span class="sxs-lookup"><span data-stu-id="67842-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="67842-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="67842-134">Request</span></span>
<span data-ttu-id="67842-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67842-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="67842-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="67842-136">Response</span></span>
<span data-ttu-id="67842-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="67842-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value"
      }
    ],
    "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
    "contributingSettings": [
      "Contributing Settings value"
    ],
    "deviceCheckinsImpacted": 6
  }
}
```





