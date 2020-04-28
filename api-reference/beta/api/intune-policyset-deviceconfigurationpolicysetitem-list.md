---
title: Список Девицеконфигуратионполицисетитемс
description: Список свойств и связей объектов Девицеконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 357177f4a89f695fd1324b48608be67014aec9be
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448721"
---
# <a name="list-deviceconfigurationpolicysetitems"></a><span data-ttu-id="de224-103">Список Девицеконфигуратионполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="de224-103">List deviceConfigurationPolicySetItems</span></span>

<span data-ttu-id="de224-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de224-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de224-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de224-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de224-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de224-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de224-107">Список свойств и связей объектов [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="de224-107">List properties and relationships of the [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de224-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de224-108">Prerequisites</span></span>
<span data-ttu-id="de224-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de224-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de224-111">Permission type</span></span>|<span data-ttu-id="de224-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de224-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de224-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de224-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de224-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de224-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="de224-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de224-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de224-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de224-116">Not supported.</span></span>|
|<span data-ttu-id="de224-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de224-117">Application</span></span>|<span data-ttu-id="de224-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de224-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de224-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de224-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="de224-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de224-120">Request headers</span></span>
|<span data-ttu-id="de224-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de224-121">Header</span></span>|<span data-ttu-id="de224-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de224-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de224-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de224-123">Authorization</span></span>|<span data-ttu-id="de224-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de224-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de224-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de224-125">Accept</span></span>|<span data-ttu-id="de224-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de224-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de224-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de224-127">Request body</span></span>
<span data-ttu-id="de224-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de224-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de224-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="de224-129">Response</span></span>
<span data-ttu-id="de224-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de224-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de224-131">Пример</span><span class="sxs-lookup"><span data-stu-id="de224-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="de224-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="de224-132">Request</span></span>
<span data-ttu-id="de224-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de224-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="de224-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="de224-134">Response</span></span>
<span data-ttu-id="de224-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de224-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
      "id": "00b1197c-197c-00b1-7c19-b1007c19b100",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```



