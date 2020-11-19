---
title: Удаление Андроидвпнконфигуратион
description: Удаляет объект Андроидвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a52a63f91bfe7dfc1f462104d9fb0efbf2ae77b6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221640"
---
# <a name="delete-androidvpnconfiguration"></a><span data-ttu-id="1d0db-103">Удаление Андроидвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1d0db-103">Delete androidVpnConfiguration</span></span>

<span data-ttu-id="1d0db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d0db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d0db-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d0db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d0db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d0db-107">Удаляет объект [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d0db-107">Deletes a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d0db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d0db-108">Prerequisites</span></span>
<span data-ttu-id="1d0db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d0db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d0db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d0db-111">Permission type</span></span>|<span data-ttu-id="1d0db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d0db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d0db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d0db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d0db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d0db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d0db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d0db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d0db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0db-116">Not supported.</span></span>|
|<span data-ttu-id="1d0db-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1d0db-117">Application</span></span>|<span data-ttu-id="1d0db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d0db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d0db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d0db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1d0db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1d0db-120">Request headers</span></span>
|<span data-ttu-id="1d0db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d0db-121">Header</span></span>|<span data-ttu-id="1d0db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d0db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d0db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d0db-123">Authorization</span></span>|<span data-ttu-id="1d0db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d0db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d0db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d0db-125">Accept</span></span>|<span data-ttu-id="1d0db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d0db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d0db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d0db-127">Request body</span></span>
<span data-ttu-id="1d0db-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d0db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d0db-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d0db-129">Response</span></span>
<span data-ttu-id="1d0db-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1d0db-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1d0db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1d0db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d0db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d0db-132">Request</span></span>
<span data-ttu-id="1d0db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d0db-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1d0db-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d0db-134">Response</span></span>
<span data-ttu-id="1d0db-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d0db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




