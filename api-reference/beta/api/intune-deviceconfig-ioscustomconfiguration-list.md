---
title: Перечисление объектов iosCustomConfiguration
description: Список свойств и связей объектов iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f2bbe98012246bfab30108fad1635370708a534
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170114"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="0bd20-103">Перечисление объектов iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="0bd20-103">List iosCustomConfigurations</span></span>

> <span data-ttu-id="0bd20-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bd20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bd20-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bd20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bd20-106">Список свойств и связей объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bd20-106">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bd20-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0bd20-107">Prerequisites</span></span>
<span data-ttu-id="0bd20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bd20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0bd20-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bd20-110">Permission type</span></span>|<span data-ttu-id="0bd20-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bd20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bd20-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bd20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bd20-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bd20-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0bd20-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bd20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bd20-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bd20-115">Not supported.</span></span>|
|<span data-ttu-id="0bd20-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bd20-116">Application</span></span>|<span data-ttu-id="0bd20-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bd20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bd20-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bd20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0bd20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bd20-119">Request headers</span></span>
|<span data-ttu-id="0bd20-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bd20-120">Header</span></span>|<span data-ttu-id="0bd20-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0bd20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bd20-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bd20-122">Authorization</span></span>|<span data-ttu-id="0bd20-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0bd20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bd20-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0bd20-124">Accept</span></span>|<span data-ttu-id="0bd20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bd20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd20-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bd20-126">Request body</span></span>
<span data-ttu-id="0bd20-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bd20-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bd20-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bd20-128">Response</span></span>
<span data-ttu-id="0bd20-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0bd20-129">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd20-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0bd20-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bd20-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bd20-131">Request</span></span>
<span data-ttu-id="0bd20-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bd20-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0bd20-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bd20-133">Response</span></span>
<span data-ttu-id="0bd20-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bd20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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




