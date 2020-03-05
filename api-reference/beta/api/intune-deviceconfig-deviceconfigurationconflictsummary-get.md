---
title: Получение Девицеконфигуратионконфликтсуммари
description: Чтение свойств и связей объекта Девицеконфигуратионконфликтсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8d5f54c9ac3d551b8cc6d149808bea2dd0911e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449182"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="efabf-103">Получение Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="efabf-103">Get deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="efabf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="efabf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efabf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efabf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efabf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efabf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efabf-107">Чтение свойств и связей объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="efabf-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efabf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="efabf-108">Prerequisites</span></span>
<span data-ttu-id="efabf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efabf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efabf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efabf-111">Permission type</span></span>|<span data-ttu-id="efabf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efabf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efabf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efabf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efabf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="efabf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="efabf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efabf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efabf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efabf-116">Not supported.</span></span>|
|<span data-ttu-id="efabf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efabf-117">Application</span></span>|<span data-ttu-id="efabf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="efabf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efabf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efabf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efabf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efabf-120">Optional query parameters</span></span>
<span data-ttu-id="efabf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="efabf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efabf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efabf-122">Request headers</span></span>
|<span data-ttu-id="efabf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efabf-123">Header</span></span>|<span data-ttu-id="efabf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="efabf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efabf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="efabf-125">Authorization</span></span>|<span data-ttu-id="efabf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efabf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efabf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="efabf-127">Accept</span></span>|<span data-ttu-id="efabf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="efabf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efabf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efabf-129">Request body</span></span>
<span data-ttu-id="efabf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efabf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efabf-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="efabf-131">Response</span></span>
<span data-ttu-id="efabf-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efabf-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efabf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="efabf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="efabf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="efabf-134">Request</span></span>
<span data-ttu-id="efabf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efabf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="efabf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="efabf-136">Response</span></span>
<span data-ttu-id="efabf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efabf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





