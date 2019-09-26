---
title: Список Виндовсдомаинжоинконфигуратионс
description: Список свойств и связей объектов Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b09361a6ddd8b520ecf83ca41e15baed59382a1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195708"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="c2fee-103">Список Виндовсдомаинжоинконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="c2fee-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="c2fee-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2fee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2fee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2fee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2fee-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2fee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2fee-107">Список свойств и связей объектов [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c2fee-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2fee-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2fee-108">Prerequisites</span></span>
<span data-ttu-id="c2fee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2fee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2fee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2fee-111">Permission type</span></span>|<span data-ttu-id="c2fee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2fee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2fee-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c2fee-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="c2fee-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c2fee-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2fee-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c2fee-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2fee-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2fee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2fee-117">Not supported.</span></span>|
|<span data-ttu-id="c2fee-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2fee-118">Application</span></span>||
| <span data-ttu-id="c2fee-119">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="c2fee-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c2fee-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2fee-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2fee-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2fee-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2fee-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2fee-122">Request headers</span></span>
|<span data-ttu-id="c2fee-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2fee-123">Header</span></span>|<span data-ttu-id="c2fee-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c2fee-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2fee-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2fee-125">Authorization</span></span>|<span data-ttu-id="c2fee-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2fee-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2fee-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c2fee-127">Accept</span></span>|<span data-ttu-id="c2fee-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2fee-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2fee-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2fee-129">Request body</span></span>
<span data-ttu-id="c2fee-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2fee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2fee-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2fee-131">Response</span></span>
<span data-ttu-id="c2fee-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2fee-132">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2fee-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2fee-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2fee-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2fee-134">Request</span></span>
<span data-ttu-id="c2fee-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2fee-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c2fee-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2fee-136">Response</span></span>
<span data-ttu-id="c2fee-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2fee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
      "id": "40118d08-8d08-4011-088d-1140088d1140",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "computerNameStaticPrefix": "Computer Name Static Prefix value",
      "computerNameSuffixRandomCharCount": 1,
      "activeDirectoryDomainName": "Active Directory Domain Name value",
      "organizationalUnit": "Organizational Unit value"
    }
  ]
}
```







