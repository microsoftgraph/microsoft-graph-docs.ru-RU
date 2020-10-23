---
title: Список Виндовсдомаинжоинконфигуратионс
description: Список свойств и связей объектов Виндовсдомаинжоинконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cd641761a53186c2dc308dfff9f1633c0a445d0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702784"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="8008f-103">Список Виндовсдомаинжоинконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="8008f-103">List windowsDomainJoinConfigurations</span></span>

<span data-ttu-id="8008f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8008f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8008f-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8008f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8008f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8008f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8008f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8008f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8008f-108">Список свойств и связей объектов [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8008f-108">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8008f-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8008f-109">Prerequisites</span></span>
<span data-ttu-id="8008f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8008f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8008f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8008f-112">Permission type</span></span>|<span data-ttu-id="8008f-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8008f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8008f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8008f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8008f-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8008f-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8008f-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8008f-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8008f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8008f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8008f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8008f-118">Not supported.</span></span>|
|<span data-ttu-id="8008f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8008f-119">Application</span></span>||
| <span data-ttu-id="8008f-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8008f-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8008f-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8008f-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8008f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8008f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8008f-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8008f-123">Request headers</span></span>
|<span data-ttu-id="8008f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8008f-124">Header</span></span>|<span data-ttu-id="8008f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8008f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8008f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8008f-126">Authorization</span></span>|<span data-ttu-id="8008f-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8008f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8008f-128">Accept</span><span class="sxs-lookup"><span data-stu-id="8008f-128">Accept</span></span>|<span data-ttu-id="8008f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8008f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8008f-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8008f-130">Request body</span></span>
<span data-ttu-id="8008f-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8008f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8008f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8008f-132">Response</span></span>
<span data-ttu-id="8008f-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8008f-133">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8008f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8008f-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8008f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8008f-135">Request</span></span>
<span data-ttu-id="8008f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8008f-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8008f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8008f-137">Response</span></span>
<span data-ttu-id="8008f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8008f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











