---
title: Get deviceManagementIntentUserState
description: Чтение свойств и связей объекта deviceManagementIntentUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 939a54cb7f07cfd8893f59b3f1d672e40aa761b6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130870"
---
# <a name="get-devicemanagementintentuserstate"></a><span data-ttu-id="6dcac-103">Get deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="6dcac-103">Get deviceManagementIntentUserState</span></span>

<span data-ttu-id="6dcac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dcac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6dcac-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dcac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dcac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6dcac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dcac-107">Чтение свойств и связей [объекта deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="6dcac-107">Read properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dcac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6dcac-108">Prerequisites</span></span>
<span data-ttu-id="6dcac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dcac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dcac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dcac-111">Permission type</span></span>|<span data-ttu-id="6dcac-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dcac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dcac-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dcac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dcac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dcac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6dcac-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dcac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dcac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dcac-116">Not supported.</span></span>|
|<span data-ttu-id="6dcac-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6dcac-117">Application</span></span>|<span data-ttu-id="6dcac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dcac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dcac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dcac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dcac-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dcac-120">Optional query parameters</span></span>
<span data-ttu-id="6dcac-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6dcac-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dcac-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dcac-122">Request headers</span></span>
|<span data-ttu-id="6dcac-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6dcac-123">Header</span></span>|<span data-ttu-id="6dcac-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6dcac-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dcac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dcac-125">Authorization</span></span>|<span data-ttu-id="6dcac-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dcac-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dcac-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6dcac-127">Accept</span></span>|<span data-ttu-id="6dcac-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6dcac-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dcac-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dcac-129">Request body</span></span>
<span data-ttu-id="6dcac-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dcac-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dcac-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dcac-131">Response</span></span>
<span data-ttu-id="6dcac-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6dcac-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dcac-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6dcac-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dcac-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dcac-134">Request</span></span>
<span data-ttu-id="6dcac-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dcac-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

### <a name="response"></a><span data-ttu-id="6dcac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dcac-136">Response</span></span>
<span data-ttu-id="6dcac-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dcac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 357

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
    "id": "0201286a-286a-0201-6a28-01026a280102",
    "userPrincipalName": "User Principal Name value",
    "userName": "User Name value",
    "deviceCount": 11,
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "state": "notApplicable"
  }
}
```




