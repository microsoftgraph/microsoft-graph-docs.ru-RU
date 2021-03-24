---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6efe6ba1b7be0ae05609e9e38da18e31d9cd2e33
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135595"
---
# <a name="assign-action"></a><span data-ttu-id="7a725-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="7a725-103">assign action</span></span>

<span data-ttu-id="7a725-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a725-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a725-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a725-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a725-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a725-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a725-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7a725-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a725-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7a725-108">Prerequisites</span></span>
<span data-ttu-id="7a725-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a725-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a725-111">Permission type</span></span>|<span data-ttu-id="7a725-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a725-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a725-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a725-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a725-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a725-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a725-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a725-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a725-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a725-116">Not supported.</span></span>|
|<span data-ttu-id="7a725-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7a725-117">Application</span></span>|<span data-ttu-id="7a725-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a725-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a725-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a725-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7a725-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a725-120">Request headers</span></span>
|<span data-ttu-id="7a725-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a725-121">Header</span></span>|<span data-ttu-id="7a725-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a725-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a725-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a725-123">Authorization</span></span>|<span data-ttu-id="7a725-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a725-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a725-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a725-125">Accept</span></span>|<span data-ttu-id="7a725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a725-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a725-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a725-127">Request body</span></span>
<span data-ttu-id="7a725-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a725-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7a725-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7a725-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7a725-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a725-130">Property</span></span>|<span data-ttu-id="7a725-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a725-131">Type</span></span>|<span data-ttu-id="7a725-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a725-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a725-133">assignments</span><span class="sxs-lookup"><span data-stu-id="7a725-133">assignments</span></span>|<span data-ttu-id="7a725-134">[коллекция embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7a725-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="7a725-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7a725-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7a725-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a725-136">Response</span></span>
<span data-ttu-id="7a725-137">В случае успешного выполнения это действие возвращает код отклика и встроенную коллекцию `200 OK` [InSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7a725-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a725-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7a725-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a725-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a725-139">Request</span></span>
<span data-ttu-id="7a725-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a725-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 456

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7a725-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a725-141">Response</span></span>
<span data-ttu-id="7a725-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a725-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




