---
title: Получение Виндовсвпнконфигуратион
description: Чтение свойств и связей объекта Виндовсвпнконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 333eb0267da25c4a6f657d0060a42a06c937cf46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32511251"
---
# <a name="get-windowsvpnconfiguration"></a><span data-ttu-id="7b627-103">Получение Виндовсвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7b627-103">Get windowsVpnConfiguration</span></span>

> <span data-ttu-id="7b627-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b627-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b627-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b627-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b627-106">Чтение свойств и связей объекта [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7b627-106">Read properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b627-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b627-107">Prerequisites</span></span>
<span data-ttu-id="7b627-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b627-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b627-110">Permission type</span></span>|<span data-ttu-id="7b627-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b627-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b627-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b627-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b627-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b627-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7b627-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b627-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b627-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b627-115">Not supported.</span></span>|
|<span data-ttu-id="7b627-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b627-116">Application</span></span>|<span data-ttu-id="7b627-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b627-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b627-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b627-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b627-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b627-119">Optional query parameters</span></span>
<span data-ttu-id="7b627-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7b627-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b627-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b627-121">Request headers</span></span>
|<span data-ttu-id="7b627-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b627-122">Header</span></span>|<span data-ttu-id="7b627-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7b627-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b627-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b627-124">Authorization</span></span>|<span data-ttu-id="7b627-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b627-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b627-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7b627-126">Accept</span></span>|<span data-ttu-id="7b627-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7b627-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b627-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b627-128">Request body</span></span>
<span data-ttu-id="7b627-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b627-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b627-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b627-130">Response</span></span>
<span data-ttu-id="7b627-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b627-131">If successful, this method returns a `200 OK` response code and [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b627-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7b627-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b627-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b627-133">Request</span></span>
<span data-ttu-id="7b627-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b627-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7b627-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b627-135">Response</span></span>
<span data-ttu-id="7b627-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b627-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsVpnConfiguration",
    "id": "0d0e69cc-69cc-0d0e-cc69-0e0dcc690e0d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "connectionName": "Connection Name value",
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s"
  }
}
```





