---
title: Получение Девицеконфигуратионконфликтсуммари
description: Чтение свойств и связей объекта Девицеконфигуратионконфликтсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c2bffcd19b7a5527e2a0a775c4a30b29ec6ac33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291759"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="13f68-103">Получение Девицеконфигуратионконфликтсуммари</span><span class="sxs-lookup"><span data-stu-id="13f68-103">Get deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="13f68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13f68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13f68-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13f68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13f68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13f68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13f68-107">Чтение свойств и связей объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="13f68-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13f68-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13f68-108">Prerequisites</span></span>
<span data-ttu-id="13f68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13f68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13f68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13f68-111">Permission type</span></span>|<span data-ttu-id="13f68-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13f68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13f68-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13f68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13f68-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13f68-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13f68-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13f68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13f68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13f68-116">Not supported.</span></span>|
|<span data-ttu-id="13f68-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13f68-117">Application</span></span>|<span data-ttu-id="13f68-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13f68-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13f68-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13f68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13f68-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13f68-120">Optional query parameters</span></span>
<span data-ttu-id="13f68-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="13f68-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13f68-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13f68-122">Request headers</span></span>
|<span data-ttu-id="13f68-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13f68-123">Header</span></span>|<span data-ttu-id="13f68-124">Значение</span><span class="sxs-lookup"><span data-stu-id="13f68-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13f68-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13f68-125">Authorization</span></span>|<span data-ttu-id="13f68-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13f68-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13f68-127">Accept</span><span class="sxs-lookup"><span data-stu-id="13f68-127">Accept</span></span>|<span data-ttu-id="13f68-128">application/json</span><span class="sxs-lookup"><span data-stu-id="13f68-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13f68-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13f68-129">Request body</span></span>
<span data-ttu-id="13f68-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13f68-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13f68-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="13f68-131">Response</span></span>
<span data-ttu-id="13f68-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13f68-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13f68-133">Пример</span><span class="sxs-lookup"><span data-stu-id="13f68-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="13f68-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="13f68-134">Request</span></span>
<span data-ttu-id="13f68-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13f68-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="13f68-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="13f68-136">Response</span></span>
<span data-ttu-id="13f68-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13f68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value",
        "sourceType": "deviceIntent"
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




