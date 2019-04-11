---
title: Получение Еасемаилпрофилеконфигуратионбасе
description: Чтение свойств и связей объекта Еасемаилпрофилеконфигуратионбасе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c73c6bd944fd5fd60f32967350e6c142c985fc4b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802795"
---
# <a name="get-easemailprofileconfigurationbase"></a><span data-ttu-id="7e836-103">Получение Еасемаилпрофилеконфигуратионбасе</span><span class="sxs-lookup"><span data-stu-id="7e836-103">Get easEmailProfileConfigurationBase</span></span>

> <span data-ttu-id="7e836-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e836-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e836-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e836-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e836-106">Чтение свойств и связей объекта [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) .</span><span class="sxs-lookup"><span data-stu-id="7e836-106">Read properties and relationships of the [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e836-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e836-107">Prerequisites</span></span>
<span data-ttu-id="7e836-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e836-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e836-110">Permission type</span></span>|<span data-ttu-id="7e836-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e836-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e836-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e836-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e836-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e836-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7e836-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e836-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e836-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e836-115">Not supported.</span></span>|
|<span data-ttu-id="7e836-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e836-116">Application</span></span>|<span data-ttu-id="7e836-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e836-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e836-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e836-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e836-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e836-119">Optional query parameters</span></span>
<span data-ttu-id="7e836-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e836-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e836-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e836-121">Request headers</span></span>
|<span data-ttu-id="7e836-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e836-122">Header</span></span>|<span data-ttu-id="7e836-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7e836-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e836-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e836-124">Authorization</span></span>|<span data-ttu-id="7e836-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e836-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e836-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7e836-126">Accept</span></span>|<span data-ttu-id="7e836-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e836-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e836-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e836-128">Request body</span></span>
<span data-ttu-id="7e836-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e836-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e836-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e836-130">Response</span></span>
<span data-ttu-id="7e836-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e836-131">If successful, this method returns a `200 OK` response code and [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e836-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7e836-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e836-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e836-133">Request</span></span>
<span data-ttu-id="7e836-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e836-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7e836-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e836-135">Response</span></span>
<span data-ttu-id="7e836-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e836-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "value": {
    "@odata.type": "#microsoft.graph.easEmailProfileConfigurationBase",
    "id": "a3f96310-6310-a3f9-1063-f9a31063f9a3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "usernameSource": "primarySmtpAddress",
    "usernameAADSource": "primarySmtpAddress",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value"
  }
}
```





