---
title: Список iosLobAppProvisioningConfigurations
description: Список свойств и связей объектов iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3e9a82886a8d16634572d1f64172d7cee5fff9e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984942"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="0cd37-103">Список iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="0cd37-103">List iosLobAppProvisioningConfigurations</span></span>

> <span data-ttu-id="0cd37-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cd37-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cd37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd37-106">Список свойств и связей объектов [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0cd37-106">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd37-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0cd37-107">Prerequisites</span></span>
<span data-ttu-id="0cd37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd37-110">Permission type</span></span>|<span data-ttu-id="0cd37-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cd37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cd37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd37-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cd37-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0cd37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cd37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd37-115">Not supported.</span></span>|
|<span data-ttu-id="0cd37-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cd37-116">Application</span></span>|<span data-ttu-id="0cd37-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cd37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0cd37-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cd37-119">Request headers</span></span>
|<span data-ttu-id="0cd37-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cd37-120">Header</span></span>|<span data-ttu-id="0cd37-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0cd37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd37-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cd37-122">Authorization</span></span>|<span data-ttu-id="0cd37-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cd37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd37-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0cd37-124">Accept</span></span>|<span data-ttu-id="0cd37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd37-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cd37-126">Request body</span></span>
<span data-ttu-id="0cd37-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0cd37-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd37-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cd37-128">Response</span></span>
<span data-ttu-id="0cd37-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cd37-129">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd37-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd37-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd37-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cd37-131">Request</span></span>
<span data-ttu-id="0cd37-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cd37-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="0cd37-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd37-133">Response</span></span>
<span data-ttu-id="0cd37-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
      "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA==",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




