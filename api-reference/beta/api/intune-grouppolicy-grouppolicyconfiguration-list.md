---
title: Список Граупполициконфигуратионс
description: Список свойств и связей объектов Граупполициконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c1d87bdb0dcb5c1af59219a8cee0f06e084cb4b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155099"
---
# <a name="list-grouppolicyconfigurations"></a><span data-ttu-id="565ae-103">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="565ae-103">List groupPolicyConfigurations</span></span>

> <span data-ttu-id="565ae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="565ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="565ae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="565ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="565ae-106">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="565ae-106">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="565ae-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="565ae-107">Prerequisites</span></span>
<span data-ttu-id="565ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="565ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="565ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="565ae-110">Permission type</span></span>|<span data-ttu-id="565ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="565ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="565ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="565ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="565ae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="565ae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="565ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="565ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="565ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="565ae-115">Not supported.</span></span>|
|<span data-ttu-id="565ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="565ae-116">Application</span></span>|<span data-ttu-id="565ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="565ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="565ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="565ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="565ae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="565ae-119">Request headers</span></span>
|<span data-ttu-id="565ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="565ae-120">Header</span></span>|<span data-ttu-id="565ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="565ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="565ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="565ae-122">Authorization</span></span>|<span data-ttu-id="565ae-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="565ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="565ae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="565ae-124">Accept</span></span>|<span data-ttu-id="565ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="565ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="565ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="565ae-126">Request body</span></span>
<span data-ttu-id="565ae-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="565ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="565ae-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="565ae-128">Response</span></span>
<span data-ttu-id="565ae-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="565ae-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="565ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="565ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="565ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="565ae-131">Request</span></span>
<span data-ttu-id="565ae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="565ae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
```

### <a name="response"></a><span data-ttu-id="565ae-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="565ae-133">Response</span></span>
<span data-ttu-id="565ae-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="565ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




