---
title: действие queryByPlatformType
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e50dfc6f8d77b3f5208f4db4dad1b0ef2f26392b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665401"
---
# <a name="querybyplatformtype-action"></a><span data-ttu-id="4f551-103">действие queryByPlatformType</span><span class="sxs-lookup"><span data-stu-id="4f551-103">queryByPlatformType action</span></span>

<span data-ttu-id="4f551-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f551-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f551-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f551-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f551-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f551-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f551-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4f551-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f551-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f551-108">Prerequisites</span></span>
<span data-ttu-id="4f551-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f551-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f551-111">Permission type</span></span>|<span data-ttu-id="4f551-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f551-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f551-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f551-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f551-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f551-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f551-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f551-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f551-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f551-116">Not supported.</span></span>|
|<span data-ttu-id="4f551-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f551-117">Application</span></span>|<span data-ttu-id="4f551-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f551-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f551-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f551-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/queryByPlatformType
```

## <a name="request-headers"></a><span data-ttu-id="4f551-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f551-120">Request headers</span></span>
|<span data-ttu-id="4f551-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f551-121">Header</span></span>|<span data-ttu-id="4f551-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f551-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f551-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f551-123">Authorization</span></span>|<span data-ttu-id="4f551-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f551-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f551-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f551-125">Accept</span></span>|<span data-ttu-id="4f551-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f551-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f551-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f551-127">Request body</span></span>
<span data-ttu-id="4f551-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f551-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4f551-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4f551-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4f551-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f551-130">Property</span></span>|<span data-ttu-id="4f551-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4f551-131">Type</span></span>|<span data-ttu-id="4f551-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4f551-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f551-133">platformType</span><span class="sxs-lookup"><span data-stu-id="4f551-133">platformType</span></span>|[<span data-ttu-id="4f551-134">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="4f551-134">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="4f551-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4f551-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4f551-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f551-136">Response</span></span>
<span data-ttu-id="4f551-137">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [коллекцию deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f551-137">If successful, this action returns a `200 OK` response code and a [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f551-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4f551-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f551-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f551-139">Request</span></span>
<span data-ttu-id="4f551-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f551-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/queryByPlatformType

Content-type: application/json
Content-length: 40

{
  "platformType": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="4f551-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f551-141">Response</span></span>
<span data-ttu-id="4f551-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f551-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 487

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileBase",
      "id": "f442dd4a-dd4a-f442-4add-42f44add42f4",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




