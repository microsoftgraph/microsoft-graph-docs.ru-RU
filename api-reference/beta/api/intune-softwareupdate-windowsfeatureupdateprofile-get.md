---
title: Получение Виндовсфеатуреупдатепрофиле
description: Чтение свойств и связей объекта Виндовсфеатуреупдатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 459c61da0b63692877e94557268b54a55ce59951
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123612"
---
# <a name="get-windowsfeatureupdateprofile"></a><span data-ttu-id="6d862-103">Получение Виндовсфеатуреупдатепрофиле</span><span class="sxs-lookup"><span data-stu-id="6d862-103">Get windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="6d862-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d862-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d862-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d862-107">Чтение свойств и связей объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6d862-107">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d862-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d862-108">Prerequisites</span></span>
<span data-ttu-id="6d862-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d862-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d862-111">Permission type</span></span>|<span data-ttu-id="6d862-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d862-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d862-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d862-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d862-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d862-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6d862-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d862-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d862-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d862-116">Not supported.</span></span>|
|<span data-ttu-id="6d862-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d862-117">Application</span></span>|<span data-ttu-id="6d862-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d862-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d862-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d862-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d862-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d862-120">Optional query parameters</span></span>
<span data-ttu-id="6d862-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6d862-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d862-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d862-122">Request headers</span></span>
|<span data-ttu-id="6d862-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d862-123">Header</span></span>|<span data-ttu-id="6d862-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6d862-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d862-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d862-125">Authorization</span></span>|<span data-ttu-id="6d862-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d862-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d862-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6d862-127">Accept</span></span>|<span data-ttu-id="6d862-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6d862-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d862-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d862-129">Request body</span></span>
<span data-ttu-id="6d862-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d862-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d862-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d862-131">Response</span></span>
<span data-ttu-id="6d862-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d862-132">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d862-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6d862-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d862-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d862-134">Request</span></span>
<span data-ttu-id="6d862-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d862-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

### <a name="response"></a><span data-ttu-id="6d862-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d862-136">Response</span></span>
<span data-ttu-id="6d862-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
    "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
    "displayName": "Display Name value",
    "description": "Description value",
    "featureUpdateVersion": "Feature Update Version value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```



