---
title: Получение Граупполиципресентатиондропдовнлист
description: Чтение свойств и связей объекта Граупполиципресентатиондропдовнлист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fe1b54ee57b33d2de7c5d78d8011270607a07a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964747"
---
# <a name="get-grouppolicypresentationdropdownlist"></a><span data-ttu-id="70fe9-103">Получение Граупполиципресентатиондропдовнлист</span><span class="sxs-lookup"><span data-stu-id="70fe9-103">Get groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="70fe9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70fe9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70fe9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70fe9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70fe9-106">Чтение свойств и связей объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="70fe9-106">Read properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70fe9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="70fe9-107">Prerequisites</span></span>
<span data-ttu-id="70fe9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70fe9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70fe9-110">Permission type</span></span>|<span data-ttu-id="70fe9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70fe9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70fe9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70fe9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70fe9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="70fe9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="70fe9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70fe9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70fe9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70fe9-115">Not supported.</span></span>|
|<span data-ttu-id="70fe9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70fe9-116">Application</span></span>|<span data-ttu-id="70fe9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70fe9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70fe9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70fe9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70fe9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70fe9-119">Optional query parameters</span></span>
<span data-ttu-id="70fe9-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70fe9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70fe9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70fe9-121">Request headers</span></span>
|<span data-ttu-id="70fe9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70fe9-122">Header</span></span>|<span data-ttu-id="70fe9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="70fe9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70fe9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70fe9-124">Authorization</span></span>|<span data-ttu-id="70fe9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70fe9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70fe9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="70fe9-126">Accept</span></span>|<span data-ttu-id="70fe9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="70fe9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70fe9-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70fe9-128">Request body</span></span>
<span data-ttu-id="70fe9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70fe9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70fe9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="70fe9-130">Response</span></span>
<span data-ttu-id="70fe9-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70fe9-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70fe9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="70fe9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="70fe9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70fe9-133">Request</span></span>
<span data-ttu-id="70fe9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70fe9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="70fe9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="70fe9-135">Response</span></span>
<span data-ttu-id="70fe9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70fe9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 655

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
    "label": "Label value",
    "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultItem": {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    },
    "items": [
      {
        "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
        "displayName": "Display Name value",
        "value": "Value value"
      }
    ],
    "required": true
  }
}
```





