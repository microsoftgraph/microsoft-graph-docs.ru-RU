---
title: Удаление Виндовсдомаинжоинконфигуратион
description: Удаляет объект Виндовсдомаинжоинконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f40e0ab74df26b66c1990c793e6e93b0c826d1c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999624"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="38f70-103">Удаление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="38f70-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="38f70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38f70-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38f70-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38f70-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f70-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38f70-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38f70-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38f70-108">Удаляет объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38f70-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38f70-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38f70-109">Prerequisites</span></span>
<span data-ttu-id="38f70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f70-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38f70-112">Permission type</span></span>|<span data-ttu-id="38f70-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38f70-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38f70-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38f70-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="38f70-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="38f70-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="38f70-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f70-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="38f70-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38f70-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38f70-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f70-118">Not supported.</span></span>|
|<span data-ttu-id="38f70-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38f70-119">Application</span></span>||
| <span data-ttu-id="38f70-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="38f70-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="38f70-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f70-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38f70-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38f70-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38f70-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38f70-123">Request headers</span></span>
|<span data-ttu-id="38f70-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38f70-124">Header</span></span>|<span data-ttu-id="38f70-125">Значение</span><span class="sxs-lookup"><span data-stu-id="38f70-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38f70-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="38f70-126">Authorization</span></span>|<span data-ttu-id="38f70-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38f70-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38f70-128">Accept</span><span class="sxs-lookup"><span data-stu-id="38f70-128">Accept</span></span>|<span data-ttu-id="38f70-129">application/json</span><span class="sxs-lookup"><span data-stu-id="38f70-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38f70-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38f70-130">Request body</span></span>
<span data-ttu-id="38f70-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38f70-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38f70-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="38f70-132">Response</span></span>
<span data-ttu-id="38f70-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="38f70-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="38f70-134">Пример</span><span class="sxs-lookup"><span data-stu-id="38f70-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="38f70-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="38f70-135">Request</span></span>
<span data-ttu-id="38f70-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38f70-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="38f70-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="38f70-137">Response</span></span>
<span data-ttu-id="38f70-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38f70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












