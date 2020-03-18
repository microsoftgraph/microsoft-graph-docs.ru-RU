---
title: Список Сиделоадингкеиес
description: Список свойств и связей объектов Сиделоадингкэй.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a51e6a7cba8916d8dd939d54450d91da8a5c4ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802715"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="326ce-103">Список Сиделоадингкеиес</span><span class="sxs-lookup"><span data-stu-id="326ce-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="326ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="326ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="326ce-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="326ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="326ce-106">Список свойств и связей объектов [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="326ce-106">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="326ce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="326ce-107">Prerequisites</span></span>
<span data-ttu-id="326ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="326ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="326ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="326ce-110">Permission type</span></span>|<span data-ttu-id="326ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="326ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="326ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="326ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="326ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="326ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="326ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="326ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="326ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="326ce-115">Not supported.</span></span>|
|<span data-ttu-id="326ce-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="326ce-116">Application</span></span>|<span data-ttu-id="326ce-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="326ce-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="326ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="326ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="326ce-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="326ce-119">Request headers</span></span>
|<span data-ttu-id="326ce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="326ce-120">Header</span></span>|<span data-ttu-id="326ce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="326ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="326ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="326ce-122">Authorization</span></span>|<span data-ttu-id="326ce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="326ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="326ce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="326ce-124">Accept</span></span>|<span data-ttu-id="326ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="326ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="326ce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="326ce-126">Request body</span></span>
<span data-ttu-id="326ce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="326ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="326ce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="326ce-128">Response</span></span>
<span data-ttu-id="326ce-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="326ce-129">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="326ce-130">Пример</span><span class="sxs-lookup"><span data-stu-id="326ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="326ce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="326ce-131">Request</span></span>
<span data-ttu-id="326ce-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="326ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="326ce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="326ce-133">Response</span></span>
<span data-ttu-id="326ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="326ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```




