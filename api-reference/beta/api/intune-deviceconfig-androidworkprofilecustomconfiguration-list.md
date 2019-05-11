---
title: Список Андроидворкпрофилекустомконфигуратионс
description: Список свойств и связей объектов Андроидворкпрофилекустомконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d80663a6712a26da1845d59f6bf0a5518a639457
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928626"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="4a4ca-103">Список Андроидворкпрофилекустомконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="4a4ca-103">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="4a4ca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a4ca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a4ca-106">Список свойств и связей объектов [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4a4ca-106">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a4ca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a4ca-107">Prerequisites</span></span>
<span data-ttu-id="4a4ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a4ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a4ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a4ca-110">Permission type</span></span>|<span data-ttu-id="4a4ca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a4ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a4ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a4ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a4ca-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a4ca-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a4ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a4ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a4ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-115">Not supported.</span></span>|
|<span data-ttu-id="4a4ca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a4ca-116">Application</span></span>|<span data-ttu-id="4a4ca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a4ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a4ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4a4ca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a4ca-119">Request headers</span></span>
|<span data-ttu-id="4a4ca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a4ca-120">Header</span></span>|<span data-ttu-id="4a4ca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a4ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a4ca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a4ca-122">Authorization</span></span>|<span data-ttu-id="4a4ca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a4ca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4a4ca-124">Accept</span></span>|<span data-ttu-id="4a4ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a4ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a4ca-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a4ca-126">Request body</span></span>
<span data-ttu-id="4a4ca-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a4ca-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a4ca-128">Response</span></span>
<span data-ttu-id="4a4ca-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a4ca-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4a4ca-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a4ca-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a4ca-131">Request</span></span>
<span data-ttu-id="4a4ca-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4a4ca-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a4ca-133">Response</span></span>
<span data-ttu-id="4a4ca-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a4ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```




