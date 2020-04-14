---
title: Удаление Виндовсдомаинжоинконфигуратион
description: Удаляет объект Виндовсдомаинжоинконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 512b039660cfda0ebe8e4bfd243dbf0a2fc25b90
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447344"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="e9690-103">Удаление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e9690-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="e9690-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9690-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9690-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9690-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e9690-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9690-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9690-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9690-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9690-108">Удаляет объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9690-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9690-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e9690-109">Prerequisites</span></span>
<span data-ttu-id="e9690-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9690-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9690-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9690-112">Permission type</span></span>|<span data-ttu-id="e9690-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9690-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9690-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9690-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e9690-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="e9690-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e9690-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9690-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="e9690-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9690-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9690-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9690-118">Not supported.</span></span>|
|<span data-ttu-id="e9690-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9690-119">Application</span></span>||
| <span data-ttu-id="e9690-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="e9690-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e9690-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9690-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9690-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9690-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e9690-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9690-123">Request headers</span></span>
|<span data-ttu-id="e9690-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9690-124">Header</span></span>|<span data-ttu-id="e9690-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e9690-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9690-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9690-126">Authorization</span></span>|<span data-ttu-id="e9690-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9690-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9690-128">Accept</span><span class="sxs-lookup"><span data-stu-id="e9690-128">Accept</span></span>|<span data-ttu-id="e9690-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e9690-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9690-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9690-130">Request body</span></span>
<span data-ttu-id="e9690-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9690-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9690-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9690-132">Response</span></span>
<span data-ttu-id="e9690-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e9690-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e9690-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e9690-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9690-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9690-135">Request</span></span>
<span data-ttu-id="e9690-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9690-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e9690-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9690-137">Response</span></span>
<span data-ttu-id="e9690-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9690-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









