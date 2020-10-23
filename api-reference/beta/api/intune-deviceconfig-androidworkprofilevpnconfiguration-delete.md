---
title: Удаление Андроидворкпрофилевпнконфигуратион
description: Удаляет объект Андроидворкпрофилевпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e1e8d54c0b8847e45ae50a1cc25d6aa93550d71
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691129"
---
# <a name="delete-androidworkprofilevpnconfiguration"></a><span data-ttu-id="2cb17-103">Удаление Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2cb17-103">Delete androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="2cb17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cb17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cb17-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cb17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cb17-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cb17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cb17-107">Удаляет объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cb17-107">Deletes a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cb17-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2cb17-108">Prerequisites</span></span>
<span data-ttu-id="2cb17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cb17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cb17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cb17-111">Permission type</span></span>|<span data-ttu-id="2cb17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cb17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cb17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cb17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cb17-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb17-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cb17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cb17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cb17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cb17-116">Not supported.</span></span>|
|<span data-ttu-id="2cb17-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cb17-117">Application</span></span>|<span data-ttu-id="2cb17-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb17-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cb17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cb17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2cb17-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2cb17-120">Request headers</span></span>
|<span data-ttu-id="2cb17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cb17-121">Header</span></span>|<span data-ttu-id="2cb17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cb17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cb17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cb17-123">Authorization</span></span>|<span data-ttu-id="2cb17-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cb17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cb17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cb17-125">Accept</span></span>|<span data-ttu-id="2cb17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cb17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cb17-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cb17-127">Request body</span></span>
<span data-ttu-id="2cb17-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cb17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cb17-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cb17-129">Response</span></span>
<span data-ttu-id="2cb17-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2cb17-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cb17-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2cb17-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cb17-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cb17-132">Request</span></span>
<span data-ttu-id="2cb17-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cb17-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2cb17-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cb17-134">Response</span></span>
<span data-ttu-id="2cb17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cb17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





