---
title: Действие extendFeatureUpdatesPause
description: Расширение функции PAUSE для центра обновления Windows для бизнеса.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: caf3d88f1a12d0e6252e946b24eedd6752ead296
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42732498"
---
# <a name="extendfeatureupdatespause-action"></a><span data-ttu-id="5a048-103">Действие extendFeatureUpdatesPause</span><span class="sxs-lookup"><span data-stu-id="5a048-103">extendFeatureUpdatesPause action</span></span>

> <span data-ttu-id="5a048-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a048-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a048-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a048-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a048-106">Расширение функции PAUSE для центра обновления Windows для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5a048-106">Extend Feature Updates Pause for a Windows Update for Business ring.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a048-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a048-107">Prerequisites</span></span>
<span data-ttu-id="5a048-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a048-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a048-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a048-110">Permission type</span></span>|<span data-ttu-id="5a048-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a048-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a048-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a048-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a048-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a048-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a048-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a048-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a048-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a048-115">Not supported.</span></span>|
|<span data-ttu-id="5a048-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5a048-116">Application</span></span>|<span data-ttu-id="5a048-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a048-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a048-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a048-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="5a048-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5a048-119">Request headers</span></span>
|<span data-ttu-id="5a048-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a048-120">Header</span></span>|<span data-ttu-id="5a048-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a048-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a048-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a048-122">Authorization</span></span>|<span data-ttu-id="5a048-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a048-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a048-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a048-124">Accept</span></span>|<span data-ttu-id="5a048-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a048-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a048-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a048-126">Request body</span></span>
<span data-ttu-id="5a048-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a048-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a048-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a048-128">Response</span></span>
<span data-ttu-id="5a048-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5a048-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5a048-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5a048-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a048-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a048-131">Request</span></span>
<span data-ttu-id="5a048-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a048-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

### <a name="response"></a><span data-ttu-id="5a048-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a048-133">Response</span></span>
<span data-ttu-id="5a048-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a048-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




