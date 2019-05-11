---
title: Получение targetedManagedAppConfiguration
description: Чтение свойств и связей объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75c753cebc5a663a3da9a9fe61f19089797b459d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33902901"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="497c4-103">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="497c4-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="497c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="497c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="497c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="497c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="497c4-106">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="497c4-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="497c4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="497c4-107">Prerequisites</span></span>
<span data-ttu-id="497c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="497c4-110">Permission type</span></span>|<span data-ttu-id="497c4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="497c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="497c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="497c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="497c4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="497c4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="497c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="497c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="497c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="497c4-115">Not supported.</span></span>|
|<span data-ttu-id="497c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="497c4-116">Application</span></span>|<span data-ttu-id="497c4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="497c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="497c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="497c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="497c4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="497c4-119">Optional query parameters</span></span>
<span data-ttu-id="497c4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="497c4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="497c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="497c4-121">Request headers</span></span>
|<span data-ttu-id="497c4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="497c4-122">Header</span></span>|<span data-ttu-id="497c4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="497c4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="497c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="497c4-124">Authorization</span></span>|<span data-ttu-id="497c4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="497c4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="497c4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="497c4-126">Accept</span></span>|<span data-ttu-id="497c4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="497c4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="497c4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="497c4-128">Request body</span></span>
<span data-ttu-id="497c4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="497c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497c4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="497c4-130">Response</span></span>
<span data-ttu-id="497c4-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="497c4-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="497c4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="497c4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="497c4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="497c4-133">Request</span></span>
<span data-ttu-id="497c4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="497c4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="497c4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="497c4-135">Response</span></span>
<span data-ttu-id="497c4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="497c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```




