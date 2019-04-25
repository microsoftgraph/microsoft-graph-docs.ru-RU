---
title: Получение ГраупполиципресентатионвалуедеЦимал
description: Чтение свойств и связей объекта ГраупполиципресентатионвалуедеЦимал.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d043822a0ac635e2eac43d4d7141ffa351ac8c02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530853"
---
# <a name="get-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="3c93e-103">Получение ГраупполиципресентатионвалуедеЦимал</span><span class="sxs-lookup"><span data-stu-id="3c93e-103">Get groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="3c93e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c93e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c93e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c93e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c93e-106">Чтение свойств и связей объекта [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="3c93e-106">Read properties and relationships of the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c93e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c93e-107">Prerequisites</span></span>
<span data-ttu-id="3c93e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c93e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c93e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c93e-110">Permission type</span></span>|<span data-ttu-id="3c93e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c93e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c93e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c93e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c93e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c93e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3c93e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c93e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c93e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c93e-115">Not supported.</span></span>|
|<span data-ttu-id="3c93e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c93e-116">Application</span></span>|<span data-ttu-id="3c93e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c93e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c93e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c93e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c93e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c93e-119">Optional query parameters</span></span>
<span data-ttu-id="3c93e-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c93e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c93e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c93e-121">Request headers</span></span>
|<span data-ttu-id="3c93e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c93e-122">Header</span></span>|<span data-ttu-id="3c93e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3c93e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c93e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c93e-124">Authorization</span></span>|<span data-ttu-id="3c93e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c93e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c93e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3c93e-126">Accept</span></span>|<span data-ttu-id="3c93e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3c93e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c93e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c93e-128">Request body</span></span>
<span data-ttu-id="3c93e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c93e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c93e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c93e-130">Response</span></span>
<span data-ttu-id="3c93e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c93e-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c93e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3c93e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c93e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c93e-133">Request</span></span>
<span data-ttu-id="3c93e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c93e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="3c93e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c93e-135">Response</span></span>
<span data-ttu-id="3c93e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c93e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "8821bede-bede-8821-debe-2188debe2188",
    "value": 5
  }
}
```





