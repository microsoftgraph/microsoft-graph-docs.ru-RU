---
title: Список Андроидворкпрофилевификонфигуратионс
description: Список свойств и связей объектов Андроидворкпрофилевификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82fc3e51d527b9e192039df65b932395c18fdfd2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975716"
---
# <a name="list-androidworkprofilewificonfigurations"></a><span data-ttu-id="7c988-103">Список Андроидворкпрофилевификонфигуратионс</span><span class="sxs-lookup"><span data-stu-id="7c988-103">List androidWorkProfileWiFiConfigurations</span></span>

> <span data-ttu-id="7c988-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c988-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c988-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c988-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c988-106">Список свойств и связей объектов [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7c988-106">List properties and relationships of the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c988-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c988-107">Prerequisites</span></span>
<span data-ttu-id="7c988-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c988-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c988-110">Permission type</span></span>|<span data-ttu-id="7c988-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c988-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c988-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c988-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c988-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c988-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c988-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c988-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c988-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c988-115">Not supported.</span></span>|
|<span data-ttu-id="7c988-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c988-116">Application</span></span>|<span data-ttu-id="7c988-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c988-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c988-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c988-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c988-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c988-119">Request headers</span></span>
|<span data-ttu-id="7c988-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c988-120">Header</span></span>|<span data-ttu-id="7c988-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c988-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c988-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c988-122">Authorization</span></span>|<span data-ttu-id="7c988-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c988-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c988-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c988-124">Accept</span></span>|<span data-ttu-id="7c988-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c988-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c988-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c988-126">Request body</span></span>
<span data-ttu-id="7c988-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c988-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c988-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c988-128">Response</span></span>
<span data-ttu-id="7c988-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c988-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c988-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7c988-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c988-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c988-131">Request</span></span>
<span data-ttu-id="7c988-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c988-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7c988-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c988-133">Response</span></span>
<span data-ttu-id="7c988-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c988-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
      "id": "8400d131-d131-8400-31d1-008431d10084",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaEnterprise"
    }
  ]
}
```




