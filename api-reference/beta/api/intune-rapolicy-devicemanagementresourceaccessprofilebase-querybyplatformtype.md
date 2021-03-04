---
title: действие queryByPlatformType
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfef02eac2586fc98f8a86f9e7740b654695e14f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447458"
---
# <a name="querybyplatformtype-action"></a><span data-ttu-id="dd4fc-103">действие queryByPlatformType</span><span class="sxs-lookup"><span data-stu-id="dd4fc-103">queryByPlatformType action</span></span>

<span data-ttu-id="dd4fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd4fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd4fc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd4fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd4fc-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd4fc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd4fc-108">Prerequisites</span></span>
<span data-ttu-id="dd4fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd4fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd4fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd4fc-111">Permission type</span></span>|<span data-ttu-id="dd4fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd4fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd4fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd4fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd4fc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd4fc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dd4fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd4fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd4fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-116">Not supported.</span></span>|
|<span data-ttu-id="dd4fc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd4fc-117">Application</span></span>|<span data-ttu-id="dd4fc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd4fc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd4fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd4fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/queryByPlatformType
```

## <a name="request-headers"></a><span data-ttu-id="dd4fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd4fc-120">Request headers</span></span>
|<span data-ttu-id="dd4fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd4fc-121">Header</span></span>|<span data-ttu-id="dd4fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd4fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd4fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd4fc-123">Authorization</span></span>|<span data-ttu-id="dd4fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd4fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd4fc-125">Accept</span></span>|<span data-ttu-id="dd4fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd4fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd4fc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd4fc-127">Request body</span></span>
<span data-ttu-id="dd4fc-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dd4fc-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dd4fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd4fc-130">Property</span></span>|<span data-ttu-id="dd4fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd4fc-131">Type</span></span>|<span data-ttu-id="dd4fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd4fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd4fc-133">platformType</span><span class="sxs-lookup"><span data-stu-id="dd4fc-133">platformType</span></span>|[<span data-ttu-id="dd4fc-134">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="dd4fc-134">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="dd4fc-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dd4fc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd4fc-136">Response</span></span>
<span data-ttu-id="dd4fc-137">В случае успешного действия возвращается код ответа `200 OK` [и iQueryable_1OfDeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-iqueryable_1ofdevicemanagementresourceaccessprofilebase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-137">If successful, this action returns a `200 OK` response code and a [iQueryable_1OfDeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-iqueryable_1ofdevicemanagementresourceaccessprofilebase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd4fc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dd4fc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd4fc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd4fc-139">Request</span></span>
<span data-ttu-id="dd4fc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/queryByPlatformType

Content-type: application/json
Content-length: 40

{
  "platformType": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="dd4fc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd4fc-141">Response</span></span>
<span data-ttu-id="dd4fc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd4fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 117

{
  "value": {
    "@odata.type": "microsoft.graph.iQueryable_1OfDeviceManagementResourceAccessProfileBase"
  }
}
```




