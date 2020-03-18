---
title: Список Виндовсдомаинжоинконфигуратионс
description: Список свойств и связей объектов Виндовсдомаинжоинконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 159338ab3596861a67b77b89c5f269767edc6bf7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800461"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="7f337-103">Список Виндовсдомаинжоинконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="7f337-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="7f337-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f337-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f337-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f337-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f337-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f337-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f337-107">Список свойств и связей объектов [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7f337-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f337-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f337-108">Prerequisites</span></span>
<span data-ttu-id="7f337-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f337-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f337-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f337-111">Permission type</span></span>|<span data-ttu-id="7f337-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f337-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f337-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f337-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7f337-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="7f337-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7f337-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f337-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f337-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f337-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f337-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f337-117">Not supported.</span></span>|
|<span data-ttu-id="7f337-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f337-118">Application</span></span>||
| <span data-ttu-id="7f337-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="7f337-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7f337-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f337-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f337-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f337-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f337-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f337-122">Request headers</span></span>
|<span data-ttu-id="7f337-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f337-123">Header</span></span>|<span data-ttu-id="7f337-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7f337-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f337-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f337-125">Authorization</span></span>|<span data-ttu-id="7f337-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f337-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f337-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7f337-127">Accept</span></span>|<span data-ttu-id="7f337-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f337-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f337-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f337-129">Request body</span></span>
<span data-ttu-id="7f337-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f337-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f337-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f337-131">Response</span></span>
<span data-ttu-id="7f337-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f337-132">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f337-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7f337-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f337-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f337-134">Request</span></span>
<span data-ttu-id="7f337-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f337-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7f337-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f337-136">Response</span></span>
<span data-ttu-id="7f337-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f337-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










