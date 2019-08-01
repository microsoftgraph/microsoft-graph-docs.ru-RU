---
title: Перечисление объектов macOSCustomConfiguration
description: Список свойств и связей объектов macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28f57cd01c4cb1c15ef6c81a820dd674163f1da1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017135"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="97d82-103">Перечисление объектов macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="97d82-103">List macOSCustomConfigurations</span></span>

> <span data-ttu-id="97d82-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97d82-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d82-105">Список свойств и связей объектов [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97d82-105">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97d82-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="97d82-106">Prerequisites</span></span>
<span data-ttu-id="97d82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97d82-109">Permission type</span></span>|<span data-ttu-id="97d82-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97d82-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97d82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97d82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97d82-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97d82-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97d82-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97d82-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97d82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d82-114">Not supported.</span></span>|
|<span data-ttu-id="97d82-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97d82-115">Application</span></span>|<span data-ttu-id="97d82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d82-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d82-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97d82-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="97d82-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97d82-118">Request headers</span></span>
|<span data-ttu-id="97d82-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97d82-119">Header</span></span>|<span data-ttu-id="97d82-120">Значение</span><span class="sxs-lookup"><span data-stu-id="97d82-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97d82-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97d82-121">Authorization</span></span>|<span data-ttu-id="97d82-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97d82-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97d82-123">Accept</span><span class="sxs-lookup"><span data-stu-id="97d82-123">Accept</span></span>|<span data-ttu-id="97d82-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97d82-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d82-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97d82-125">Request body</span></span>
<span data-ttu-id="97d82-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97d82-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97d82-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="97d82-127">Response</span></span>
<span data-ttu-id="97d82-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97d82-128">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d82-129">Пример</span><span class="sxs-lookup"><span data-stu-id="97d82-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="97d82-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="97d82-130">Request</span></span>
<span data-ttu-id="97d82-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97d82-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="97d82-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d82-132">Response</span></span>
<span data-ttu-id="97d82-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97d82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
      "id": "a253835d-835d-a253-5d83-53a25d8353a2",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```



