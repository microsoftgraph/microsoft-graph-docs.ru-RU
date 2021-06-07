---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00d0413149350224d9fcf75bebe25ca5857b545f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745319"
---
# <a name="assign-action"></a><span data-ttu-id="23919-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="23919-103">assign action</span></span>

<span data-ttu-id="23919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23919-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23919-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23919-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="23919-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23919-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="23919-107">Prerequisites</span></span>
<span data-ttu-id="23919-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23919-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23919-110">Permission type</span></span>|<span data-ttu-id="23919-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23919-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23919-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23919-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23919-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23919-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23919-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23919-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23919-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23919-115">Not supported.</span></span>|
|<span data-ttu-id="23919-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="23919-116">Application</span></span>|<span data-ttu-id="23919-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23919-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23919-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23919-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="23919-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="23919-119">Request headers</span></span>
|<span data-ttu-id="23919-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23919-120">Header</span></span>|<span data-ttu-id="23919-121">Значение</span><span class="sxs-lookup"><span data-stu-id="23919-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23919-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23919-122">Authorization</span></span>|<span data-ttu-id="23919-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23919-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23919-124">Accept</span><span class="sxs-lookup"><span data-stu-id="23919-124">Accept</span></span>|<span data-ttu-id="23919-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23919-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23919-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23919-126">Request body</span></span>
<span data-ttu-id="23919-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23919-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="23919-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="23919-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="23919-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="23919-129">Property</span></span>|<span data-ttu-id="23919-130">Тип</span><span class="sxs-lookup"><span data-stu-id="23919-130">Type</span></span>|<span data-ttu-id="23919-131">Описание</span><span class="sxs-lookup"><span data-stu-id="23919-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23919-132">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="23919-132">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="23919-133">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="23919-133">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="23919-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="23919-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="23919-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="23919-135">Response</span></span>
<span data-ttu-id="23919-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23919-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23919-137">Пример</span><span class="sxs-lookup"><span data-stu-id="23919-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="23919-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="23919-138">Request</span></span>
<span data-ttu-id="23919-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23919-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

Content-type: application/json
Content-length: 360

{
  "enrollmentConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="23919-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="23919-140">Response</span></span>
<span data-ttu-id="23919-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23919-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




