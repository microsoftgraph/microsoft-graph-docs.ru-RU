---
title: Удаление windowsDomainJoinConfiguration
description: Удаляет windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d99fd2971efb3330d370af6cad99b8137f689ce
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866960"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="69119-103">Удаление windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="69119-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="69119-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69119-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69119-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="69119-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69119-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69119-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69119-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69119-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69119-108">Удаляет [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69119-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69119-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69119-109">Prerequisites</span></span>
<span data-ttu-id="69119-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69119-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69119-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69119-112">Permission type</span></span>|<span data-ttu-id="69119-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69119-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69119-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69119-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="69119-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="69119-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="69119-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69119-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="69119-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69119-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69119-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69119-118">Not supported.</span></span>|
|<span data-ttu-id="69119-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="69119-119">Application</span></span>||
| <span data-ttu-id="69119-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="69119-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="69119-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69119-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69119-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69119-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="69119-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69119-123">Request headers</span></span>
|<span data-ttu-id="69119-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69119-124">Header</span></span>|<span data-ttu-id="69119-125">Значение</span><span class="sxs-lookup"><span data-stu-id="69119-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69119-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69119-126">Authorization</span></span>|<span data-ttu-id="69119-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69119-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69119-128">Accept</span><span class="sxs-lookup"><span data-stu-id="69119-128">Accept</span></span>|<span data-ttu-id="69119-129">application/json</span><span class="sxs-lookup"><span data-stu-id="69119-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69119-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69119-130">Request body</span></span>
<span data-ttu-id="69119-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69119-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69119-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="69119-132">Response</span></span>
<span data-ttu-id="69119-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69119-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="69119-134">Пример</span><span class="sxs-lookup"><span data-stu-id="69119-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="69119-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="69119-135">Request</span></span>
<span data-ttu-id="69119-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69119-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="69119-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="69119-137">Response</span></span>
<span data-ttu-id="69119-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69119-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










