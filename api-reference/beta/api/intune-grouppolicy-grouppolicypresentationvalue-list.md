---
title: Список Граупполиципресентатионвалуес
description: Список свойств и связей объектов Граупполиципресентатионвалуе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6beccf67d5bf80f56ab5c8ebe9a66335e1b925f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984834"
---
# <a name="list-grouppolicypresentationvalues"></a><span data-ttu-id="de0ec-103">Список Граупполиципресентатионвалуес</span><span class="sxs-lookup"><span data-stu-id="de0ec-103">List groupPolicyPresentationValues</span></span>

> <span data-ttu-id="de0ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de0ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de0ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de0ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de0ec-106">Список свойств и связей объектов [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="de0ec-106">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de0ec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de0ec-107">Prerequisites</span></span>
<span data-ttu-id="de0ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de0ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de0ec-110">Permission type</span></span>|<span data-ttu-id="de0ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de0ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de0ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de0ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de0ec-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="de0ec-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="de0ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de0ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de0ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de0ec-115">Not supported.</span></span>|
|<span data-ttu-id="de0ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de0ec-116">Application</span></span>|<span data-ttu-id="de0ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de0ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de0ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de0ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="de0ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de0ec-119">Request headers</span></span>
|<span data-ttu-id="de0ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de0ec-120">Header</span></span>|<span data-ttu-id="de0ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de0ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de0ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de0ec-122">Authorization</span></span>|<span data-ttu-id="de0ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de0ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de0ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de0ec-124">Accept</span></span>|<span data-ttu-id="de0ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de0ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de0ec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de0ec-126">Request body</span></span>
<span data-ttu-id="de0ec-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de0ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de0ec-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="de0ec-128">Response</span></span>
<span data-ttu-id="de0ec-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de0ec-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de0ec-130">Пример</span><span class="sxs-lookup"><span data-stu-id="de0ec-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="de0ec-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="de0ec-131">Request</span></span>
<span data-ttu-id="de0ec-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de0ec-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="de0ec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="de0ec-133">Response</span></span>
<span data-ttu-id="de0ec-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de0ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "8132eaab-eaab-8132-abea-3281abea3281"
    }
  ]
}
```





