---
title: Удаление Андроидвпнконфигуратион
description: Удаляет объект Андроидвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32ab3c92a4c2b8a49a9a4d1a5edf194b93e71ad9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43343939"
---
# <a name="delete-androidvpnconfiguration"></a><span data-ttu-id="10dfd-103">Удаление Андроидвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="10dfd-103">Delete androidVpnConfiguration</span></span>

<span data-ttu-id="10dfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10dfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10dfd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10dfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10dfd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10dfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10dfd-107">Удаляет объект [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10dfd-107">Deletes a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10dfd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10dfd-108">Prerequisites</span></span>
<span data-ttu-id="10dfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10dfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10dfd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10dfd-111">Permission type</span></span>|<span data-ttu-id="10dfd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10dfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10dfd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10dfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10dfd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10dfd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10dfd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10dfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10dfd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10dfd-116">Not supported.</span></span>|
|<span data-ttu-id="10dfd-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="10dfd-117">Application</span></span>|<span data-ttu-id="10dfd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10dfd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10dfd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10dfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="10dfd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="10dfd-120">Request headers</span></span>
|<span data-ttu-id="10dfd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10dfd-121">Header</span></span>|<span data-ttu-id="10dfd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="10dfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10dfd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10dfd-123">Authorization</span></span>|<span data-ttu-id="10dfd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10dfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10dfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10dfd-125">Accept</span></span>|<span data-ttu-id="10dfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10dfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10dfd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10dfd-127">Request body</span></span>
<span data-ttu-id="10dfd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10dfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10dfd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="10dfd-129">Response</span></span>
<span data-ttu-id="10dfd-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="10dfd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="10dfd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="10dfd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="10dfd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="10dfd-132">Request</span></span>
<span data-ttu-id="10dfd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10dfd-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="10dfd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="10dfd-134">Response</span></span>
<span data-ttu-id="10dfd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10dfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



