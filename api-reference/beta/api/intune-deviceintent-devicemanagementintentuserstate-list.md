---
title: Список Девицеманажементинтентусерстатес
description: Список свойств и связей объектов Девицеманажементинтентусерстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 222e41f1739eaaca7237e13d8fc7b41d93a21bfd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275141"
---
# <a name="list-devicemanagementintentuserstates"></a><span data-ttu-id="50468-103">Список Девицеманажементинтентусерстатес</span><span class="sxs-lookup"><span data-stu-id="50468-103">List deviceManagementIntentUserStates</span></span>

<span data-ttu-id="50468-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50468-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50468-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50468-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50468-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50468-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50468-107">Список свойств и связей объектов [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="50468-107">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50468-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50468-108">Prerequisites</span></span>
<span data-ttu-id="50468-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50468-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50468-111">Permission type</span></span>|<span data-ttu-id="50468-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50468-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50468-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50468-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50468-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50468-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50468-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50468-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50468-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50468-116">Not supported.</span></span>|
|<span data-ttu-id="50468-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50468-117">Application</span></span>|<span data-ttu-id="50468-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50468-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50468-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50468-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="50468-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50468-120">Request headers</span></span>
|<span data-ttu-id="50468-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50468-121">Header</span></span>|<span data-ttu-id="50468-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50468-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50468-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50468-123">Authorization</span></span>|<span data-ttu-id="50468-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50468-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50468-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50468-125">Accept</span></span>|<span data-ttu-id="50468-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50468-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50468-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50468-127">Request body</span></span>
<span data-ttu-id="50468-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50468-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50468-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="50468-129">Response</span></span>
<span data-ttu-id="50468-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50468-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50468-131">Пример</span><span class="sxs-lookup"><span data-stu-id="50468-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="50468-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="50468-132">Request</span></span>
<span data-ttu-id="50468-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50468-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
```

### <a name="response"></a><span data-ttu-id="50468-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="50468-134">Response</span></span>
<span data-ttu-id="50468-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50468-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




