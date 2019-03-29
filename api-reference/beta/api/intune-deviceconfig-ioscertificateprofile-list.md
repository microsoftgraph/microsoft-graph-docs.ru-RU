---
title: Перечисление объектов iosCertificateProfile
description: Список свойств и связей объектов iosCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c1e5194150e3e687d78784003d82691388fd01a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964677"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="8a2c4-103">Перечисление объектов iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8a2c4-103">List iosCertificateProfiles</span></span>

> <span data-ttu-id="8a2c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a2c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a2c4-106">Список свойств и связей объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8a2c4-106">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a2c4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8a2c4-107">Prerequisites</span></span>
<span data-ttu-id="8a2c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a2c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a2c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a2c4-110">Permission type</span></span>|<span data-ttu-id="8a2c4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a2c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a2c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a2c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a2c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a2c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8a2c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a2c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a2c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-115">Not supported.</span></span>|
|<span data-ttu-id="8a2c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a2c4-116">Application</span></span>|<span data-ttu-id="8a2c4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a2c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a2c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8a2c4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a2c4-119">Request headers</span></span>
|<span data-ttu-id="8a2c4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a2c4-120">Header</span></span>|<span data-ttu-id="8a2c4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8a2c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a2c4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a2c4-122">Authorization</span></span>|<span data-ttu-id="8a2c4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a2c4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8a2c4-124">Accept</span></span>|<span data-ttu-id="8a2c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a2c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a2c4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a2c4-126">Request body</span></span>
<span data-ttu-id="8a2c4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a2c4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a2c4-128">Response</span></span>
<span data-ttu-id="8a2c4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-129">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a2c4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8a2c4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a2c4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a2c4-131">Request</span></span>
<span data-ttu-id="8a2c4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8a2c4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a2c4-133">Response</span></span>
<span data-ttu-id="8a2c4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




