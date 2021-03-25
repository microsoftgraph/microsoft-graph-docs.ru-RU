---
title: List groupPolicyPresentationDropdownLists
description: Список свойств и связей объектов groupPolicyPresentationDropdownList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 033a8209959c99c638d59f919a613c504e3c2802
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157424"
---
# <a name="list-grouppolicypresentationdropdownlists"></a><span data-ttu-id="0c67a-103">List groupPolicyPresentationDropdownLists</span><span class="sxs-lookup"><span data-stu-id="0c67a-103">List groupPolicyPresentationDropdownLists</span></span>

<span data-ttu-id="0c67a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c67a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c67a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c67a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c67a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c67a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c67a-107">Список свойств и связей объектов [groupPolicyPresentationDropdownList.](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)</span><span class="sxs-lookup"><span data-stu-id="0c67a-107">List properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c67a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c67a-108">Prerequisites</span></span>
<span data-ttu-id="0c67a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c67a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c67a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c67a-111">Permission type</span></span>|<span data-ttu-id="0c67a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c67a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c67a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c67a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c67a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c67a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c67a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c67a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c67a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c67a-116">Not supported.</span></span>|
|<span data-ttu-id="0c67a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c67a-117">Application</span></span>|<span data-ttu-id="0c67a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c67a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c67a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c67a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0c67a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c67a-120">Request headers</span></span>
|<span data-ttu-id="0c67a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c67a-121">Header</span></span>|<span data-ttu-id="0c67a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c67a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c67a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c67a-123">Authorization</span></span>|<span data-ttu-id="0c67a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c67a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c67a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c67a-125">Accept</span></span>|<span data-ttu-id="0c67a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c67a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c67a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c67a-127">Request body</span></span>
<span data-ttu-id="0c67a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c67a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c67a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c67a-129">Response</span></span>
<span data-ttu-id="0c67a-130">В случае успешного завершения этот метод возвращает код ответа и коллекцию объектов `200 OK` [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c67a-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c67a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0c67a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c67a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c67a-132">Request</span></span>
<span data-ttu-id="0c67a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c67a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="0c67a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c67a-134">Response</span></span>
<span data-ttu-id="0c67a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c67a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 703

{
  "value": [
    {
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
  ]
}
```




