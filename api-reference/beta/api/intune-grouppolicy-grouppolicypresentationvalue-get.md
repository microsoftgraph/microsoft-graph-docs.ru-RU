---
title: Получение Граупполиципресентатионвалуе
description: Чтение свойств и связей объекта Граупполиципресентатионвалуе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5b265db57d9c29fe421806a0c58d412eea92023
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772141"
---
# <a name="get-grouppolicypresentationvalue"></a><span data-ttu-id="72411-103">Получение Граупполиципресентатионвалуе</span><span class="sxs-lookup"><span data-stu-id="72411-103">Get groupPolicyPresentationValue</span></span>

> <span data-ttu-id="72411-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72411-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72411-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72411-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72411-106">Чтение свойств и связей объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="72411-106">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72411-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72411-107">Prerequisites</span></span>
<span data-ttu-id="72411-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72411-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72411-110">Permission type</span></span>|<span data-ttu-id="72411-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72411-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72411-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72411-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72411-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72411-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="72411-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72411-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72411-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72411-115">Not supported.</span></span>|
|<span data-ttu-id="72411-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72411-116">Application</span></span>|<span data-ttu-id="72411-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72411-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72411-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72411-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72411-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72411-119">Optional query parameters</span></span>
<span data-ttu-id="72411-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72411-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72411-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72411-121">Request headers</span></span>
|<span data-ttu-id="72411-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72411-122">Header</span></span>|<span data-ttu-id="72411-123">Значение</span><span class="sxs-lookup"><span data-stu-id="72411-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72411-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72411-124">Authorization</span></span>|<span data-ttu-id="72411-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72411-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72411-126">Accept</span><span class="sxs-lookup"><span data-stu-id="72411-126">Accept</span></span>|<span data-ttu-id="72411-127">application/json</span><span class="sxs-lookup"><span data-stu-id="72411-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72411-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72411-128">Request body</span></span>
<span data-ttu-id="72411-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72411-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72411-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="72411-130">Response</span></span>
<span data-ttu-id="72411-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72411-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72411-132">Пример</span><span class="sxs-lookup"><span data-stu-id="72411-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="72411-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="72411-133">Request</span></span>
<span data-ttu-id="72411-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72411-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="72411-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="72411-135">Response</span></span>
<span data-ttu-id="72411-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72411-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "8132eaab-eaab-8132-abea-3281abea3281"
  }
}
```





