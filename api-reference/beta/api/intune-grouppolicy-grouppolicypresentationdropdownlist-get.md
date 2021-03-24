---
title: Get groupPolicyPresentationDropdownList
description: Чтение свойств и связей объекта groupPolicyPresentationDropdownList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67fc39f11bc484e6aaa0bad4bac1391a2a533eb8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149578"
---
# <a name="get-grouppolicypresentationdropdownlist"></a><span data-ttu-id="c5610-103">Get groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="c5610-103">Get groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="c5610-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5610-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5610-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5610-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5610-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5610-107">Чтение свойств и связей объекта [groupPolicyPresentationDropdownList.](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)</span><span class="sxs-lookup"><span data-stu-id="c5610-107">Read properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5610-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5610-108">Prerequisites</span></span>
<span data-ttu-id="c5610-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5610-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5610-111">Permission type</span></span>|<span data-ttu-id="c5610-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5610-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5610-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5610-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5610-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5610-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5610-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5610-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5610-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5610-116">Not supported.</span></span>|
|<span data-ttu-id="c5610-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c5610-117">Application</span></span>|<span data-ttu-id="c5610-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5610-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5610-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5610-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5610-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5610-120">Optional query parameters</span></span>
<span data-ttu-id="c5610-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5610-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5610-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5610-122">Request headers</span></span>
|<span data-ttu-id="c5610-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5610-123">Header</span></span>|<span data-ttu-id="c5610-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c5610-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5610-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5610-125">Authorization</span></span>|<span data-ttu-id="c5610-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5610-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5610-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c5610-127">Accept</span></span>|<span data-ttu-id="c5610-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c5610-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5610-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5610-129">Request body</span></span>
<span data-ttu-id="c5610-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5610-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5610-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5610-131">Response</span></span>
<span data-ttu-id="c5610-132">В случае успешного завершения этот метод возвращает код ответа и `200 OK` [объект GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5610-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5610-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c5610-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5610-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5610-134">Request</span></span>
<span data-ttu-id="c5610-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5610-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="c5610-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5610-136">Response</span></span>
<span data-ttu-id="c5610-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5610-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




