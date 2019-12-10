---
title: Удаление Виндовсдомаинжоинконфигуратион
description: Удаляет объект Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bca34e9723df4150e3f0da5183162c385572006f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939383"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="5587a-103">Удаление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5587a-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="5587a-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5587a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5587a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5587a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5587a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5587a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5587a-107">Удаляет объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5587a-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5587a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5587a-108">Prerequisites</span></span>
<span data-ttu-id="5587a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5587a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5587a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5587a-111">Permission type</span></span>|<span data-ttu-id="5587a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5587a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5587a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5587a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5587a-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5587a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5587a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5587a-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="5587a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5587a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5587a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5587a-117">Not supported.</span></span>|
|<span data-ttu-id="5587a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5587a-118">Application</span></span>||
| <span data-ttu-id="5587a-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5587a-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5587a-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5587a-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5587a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5587a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5587a-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5587a-122">Request headers</span></span>
|<span data-ttu-id="5587a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5587a-123">Header</span></span>|<span data-ttu-id="5587a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5587a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5587a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5587a-125">Authorization</span></span>|<span data-ttu-id="5587a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5587a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5587a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5587a-127">Accept</span></span>|<span data-ttu-id="5587a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5587a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5587a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5587a-129">Request body</span></span>
<span data-ttu-id="5587a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5587a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5587a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5587a-131">Response</span></span>
<span data-ttu-id="5587a-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5587a-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5587a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5587a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5587a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5587a-134">Request</span></span>
<span data-ttu-id="5587a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5587a-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5587a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5587a-136">Response</span></span>
<span data-ttu-id="5587a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5587a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











