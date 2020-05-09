---
title: Список Девицеманажементтемплатес
description: Список свойств и связей объектов Девицеманажементтемплате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: badd561f37fda4c098bc13b99ce06b2f3c5067c4
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177200"
---
# <a name="list-devicemanagementtemplates"></a><span data-ttu-id="45754-103">Список Девицеманажементтемплатес</span><span class="sxs-lookup"><span data-stu-id="45754-103">List deviceManagementTemplates</span></span>

<span data-ttu-id="45754-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45754-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45754-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45754-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45754-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45754-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45754-107">Список свойств и связей объектов [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="45754-107">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45754-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45754-108">Prerequisites</span></span>
<span data-ttu-id="45754-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45754-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45754-111">Permission type</span></span>|<span data-ttu-id="45754-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45754-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45754-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45754-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45754-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45754-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45754-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45754-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45754-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45754-116">Not supported.</span></span>|
|<span data-ttu-id="45754-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45754-117">Application</span></span>|<span data-ttu-id="45754-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45754-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45754-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45754-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="45754-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45754-120">Request headers</span></span>
|<span data-ttu-id="45754-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45754-121">Header</span></span>|<span data-ttu-id="45754-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45754-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45754-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45754-123">Authorization</span></span>|<span data-ttu-id="45754-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45754-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45754-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45754-125">Accept</span></span>|<span data-ttu-id="45754-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45754-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45754-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45754-127">Request body</span></span>
<span data-ttu-id="45754-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45754-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45754-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="45754-129">Response</span></span>
<span data-ttu-id="45754-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45754-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45754-131">Пример</span><span class="sxs-lookup"><span data-stu-id="45754-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45754-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45754-132">Request</span></span>
<span data-ttu-id="45754-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45754-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="45754-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="45754-134">Response</span></span>
<span data-ttu-id="45754-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45754-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplate",
      "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "specializedDevices",
      "platformType": "androidForWork",
      "templateSubtype": "firewall",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
    }
  ]
}
```



