---
title: Список Андроидворкпрофилегмаилеасконфигуратионс
description: Список свойств и связей объектов Андроидворкпрофилегмаилеасконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24beedcc74d76112cd292c766b15741145faa375
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805742"
---
# <a name="list-androidworkprofilegmaileasconfigurations"></a><span data-ttu-id="9b4e8-103">Список Андроидворкпрофилегмаилеасконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="9b4e8-103">List androidWorkProfileGmailEasConfigurations</span></span>

> <span data-ttu-id="9b4e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b4e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b4e8-106">Список свойств и связей объектов [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9b4e8-106">List properties and relationships of the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b4e8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b4e8-107">Prerequisites</span></span>
<span data-ttu-id="9b4e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b4e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b4e8-110">Permission type</span></span>|<span data-ttu-id="9b4e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b4e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b4e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b4e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b4e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b4e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b4e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b4e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b4e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-115">Not supported.</span></span>|
|<span data-ttu-id="9b4e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b4e8-116">Application</span></span>|<span data-ttu-id="9b4e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b4e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b4e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9b4e8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b4e8-119">Request headers</span></span>
|<span data-ttu-id="9b4e8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b4e8-120">Header</span></span>|<span data-ttu-id="9b4e8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9b4e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b4e8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b4e8-122">Authorization</span></span>|<span data-ttu-id="9b4e8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b4e8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9b4e8-124">Accept</span></span>|<span data-ttu-id="9b4e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b4e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4e8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b4e8-126">Request body</span></span>
<span data-ttu-id="9b4e8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b4e8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b4e8-128">Response</span></span>
<span data-ttu-id="9b4e8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4e8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9b4e8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b4e8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b4e8-131">Request</span></span>
<span data-ttu-id="9b4e8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9b4e8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b4e8-133">Response</span></span>
<span data-ttu-id="9b4e8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b4e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
      "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "authenticationMethod": "certificate",
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "hostName": "Host Name value",
      "requireSsl": true,
      "usernameSource": "userPrincipalName"
    }
  ]
}
```





