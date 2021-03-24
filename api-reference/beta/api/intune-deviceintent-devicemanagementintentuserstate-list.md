---
title: Список deviceManagementIntentUserStates
description: Список свойств и связей объектов deviceManagementIntentUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 944c18beae15a484d9dc49c5c99b493a8dfef513
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127104"
---
# <a name="list-devicemanagementintentuserstates"></a><span data-ttu-id="66d27-103">Список deviceManagementIntentUserStates</span><span class="sxs-lookup"><span data-stu-id="66d27-103">List deviceManagementIntentUserStates</span></span>

<span data-ttu-id="66d27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66d27-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66d27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66d27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d27-107">Список свойств и связей [объектов deviceManagementIntentUserState.](../resources/intune-deviceintent-devicemanagementintentuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="66d27-107">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66d27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="66d27-108">Prerequisites</span></span>
<span data-ttu-id="66d27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66d27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66d27-111">Permission type</span></span>|<span data-ttu-id="66d27-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66d27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66d27-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66d27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66d27-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d27-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66d27-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66d27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66d27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66d27-116">Not supported.</span></span>|
|<span data-ttu-id="66d27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="66d27-117">Application</span></span>|<span data-ttu-id="66d27-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d27-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66d27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66d27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="66d27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66d27-120">Request headers</span></span>
|<span data-ttu-id="66d27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66d27-121">Header</span></span>|<span data-ttu-id="66d27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66d27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66d27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d27-123">Authorization</span></span>|<span data-ttu-id="66d27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66d27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66d27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66d27-125">Accept</span></span>|<span data-ttu-id="66d27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66d27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66d27-127">Request body</span></span>
<span data-ttu-id="66d27-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66d27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66d27-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="66d27-129">Response</span></span>
<span data-ttu-id="66d27-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="66d27-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d27-131">Пример</span><span class="sxs-lookup"><span data-stu-id="66d27-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="66d27-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="66d27-132">Request</span></span>
<span data-ttu-id="66d27-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66d27-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
```

### <a name="response"></a><span data-ttu-id="66d27-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="66d27-134">Response</span></span>
<span data-ttu-id="66d27-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66d27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
      "id": "0201286a-286a-0201-6a28-01026a280102",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceCount": 11,
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable"
    }
  ]
}
```




