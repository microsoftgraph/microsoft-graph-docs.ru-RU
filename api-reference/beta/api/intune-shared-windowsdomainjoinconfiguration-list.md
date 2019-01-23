---
title: Список windowsDomainJoinConfigurations
description: Свойства списка и связей объектов windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19f4687039e2a07b32994d855f3e215da2af85c8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392999"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="a4d4d-103">Список windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="a4d4d-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="a4d4d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a4d4d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4d4d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4d4d-107">Свойства списка и связей объектов [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a4d4d-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4d4d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a4d4d-108">Prerequisites</span></span>
<span data-ttu-id="a4d4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4d4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4d4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4d4d-111">Permission type</span></span>|<span data-ttu-id="a4d4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4d4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4d4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4d4d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a4d4d-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="a4d4d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a4d4d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4d4d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a4d4d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4d4d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d4d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-117">Not supported.</span></span>|
|<span data-ttu-id="a4d4d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4d4d-118">Application</span></span>|<span data-ttu-id="a4d4d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d4d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4d4d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4d4d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4d4d-121">Request headers</span></span>
|<span data-ttu-id="a4d4d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4d4d-122">Header</span></span>|<span data-ttu-id="a4d4d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a4d4d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4d4d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d4d-124">Authorization</span></span>|<span data-ttu-id="a4d4d-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a4d4d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4d4d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a4d4d-126">Accept</span></span>|<span data-ttu-id="a4d4d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a4d4d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d4d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4d4d-128">Request body</span></span>
<span data-ttu-id="a4d4d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4d4d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4d4d-130">Response</span></span>
<span data-ttu-id="a4d4d-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4d4d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a4d4d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4d4d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4d4d-133">Request</span></span>
<span data-ttu-id="a4d4d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a4d4d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4d4d-135">Response</span></span>
<span data-ttu-id="a4d4d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a4d4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



