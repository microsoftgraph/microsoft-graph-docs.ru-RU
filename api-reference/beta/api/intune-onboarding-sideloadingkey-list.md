---
title: Список Сиделоадингкеиес
description: Список свойств и связей объектов Сиделоадингкэй.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b18da0d1d5c5da63007f489708938cefb9dd51f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352409"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="5e701-103">Список Сиделоадингкеиес</span><span class="sxs-lookup"><span data-stu-id="5e701-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="5e701-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e701-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e701-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e701-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e701-106">Список свойств и связей объектов [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="5e701-106">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e701-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e701-107">Prerequisites</span></span>
<span data-ttu-id="5e701-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e701-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e701-110">Permission type</span></span>|<span data-ttu-id="5e701-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e701-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e701-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e701-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e701-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e701-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5e701-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e701-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e701-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e701-115">Not supported.</span></span>|
|<span data-ttu-id="5e701-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e701-116">Application</span></span>|<span data-ttu-id="5e701-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e701-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e701-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e701-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="5e701-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e701-119">Request headers</span></span>
|<span data-ttu-id="5e701-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e701-120">Header</span></span>|<span data-ttu-id="5e701-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5e701-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e701-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e701-122">Authorization</span></span>|<span data-ttu-id="5e701-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e701-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e701-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5e701-124">Accept</span></span>|<span data-ttu-id="5e701-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e701-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e701-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e701-126">Request body</span></span>
<span data-ttu-id="5e701-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e701-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e701-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e701-128">Response</span></span>
<span data-ttu-id="5e701-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e701-129">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e701-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5e701-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e701-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e701-131">Request</span></span>
<span data-ttu-id="5e701-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e701-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="5e701-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e701-133">Response</span></span>
<span data-ttu-id="5e701-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e701-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






