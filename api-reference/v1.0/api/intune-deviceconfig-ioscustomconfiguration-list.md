---
title: Перечисление объектов iosCustomConfiguration
description: Список свойств и связей объектов iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0bbdd104a7f614bb86e143ce3cec2a4fadfcb9a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984578"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="30fff-103">Перечисление объектов iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="30fff-103">List iosCustomConfigurations</span></span>

> <span data-ttu-id="30fff-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30fff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30fff-105">Список свойств и связей объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30fff-105">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30fff-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30fff-106">Prerequisites</span></span>
<span data-ttu-id="30fff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30fff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30fff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30fff-109">Permission type</span></span>|<span data-ttu-id="30fff-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30fff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30fff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30fff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30fff-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30fff-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30fff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30fff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30fff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30fff-114">Not supported.</span></span>|
|<span data-ttu-id="30fff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30fff-115">Application</span></span>|<span data-ttu-id="30fff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30fff-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30fff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30fff-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="30fff-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30fff-118">Request headers</span></span>
|<span data-ttu-id="30fff-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30fff-119">Header</span></span>|<span data-ttu-id="30fff-120">Значение</span><span class="sxs-lookup"><span data-stu-id="30fff-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30fff-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30fff-121">Authorization</span></span>|<span data-ttu-id="30fff-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30fff-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30fff-123">Accept</span><span class="sxs-lookup"><span data-stu-id="30fff-123">Accept</span></span>|<span data-ttu-id="30fff-124">application/json</span><span class="sxs-lookup"><span data-stu-id="30fff-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30fff-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30fff-125">Request body</span></span>
<span data-ttu-id="30fff-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30fff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30fff-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="30fff-127">Response</span></span>
<span data-ttu-id="30fff-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30fff-128">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30fff-129">Пример</span><span class="sxs-lookup"><span data-stu-id="30fff-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="30fff-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="30fff-130">Request</span></span>
<span data-ttu-id="30fff-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30fff-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="30fff-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="30fff-132">Response</span></span>
<span data-ttu-id="30fff-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30fff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 524

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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



