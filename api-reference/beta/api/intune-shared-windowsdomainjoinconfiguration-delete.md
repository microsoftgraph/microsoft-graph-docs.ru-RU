---
title: Удаление Виндовсдомаинжоинконфигуратион
description: Удаляет объект Виндовсдомаинжоинконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53a9d06cc36ecba3499d25f336aa3dc2a8521ccd
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195715"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="2adcf-103">Удаление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2adcf-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="2adcf-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2adcf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2adcf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2adcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2adcf-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2adcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2adcf-107">Удаляет объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2adcf-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2adcf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2adcf-108">Prerequisites</span></span>
<span data-ttu-id="2adcf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2adcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2adcf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2adcf-111">Permission type</span></span>|<span data-ttu-id="2adcf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2adcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2adcf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2adcf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2adcf-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="2adcf-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2adcf-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2adcf-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="2adcf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2adcf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2adcf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2adcf-117">Not supported.</span></span>|
|<span data-ttu-id="2adcf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2adcf-118">Application</span></span>||
| <span data-ttu-id="2adcf-119">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="2adcf-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2adcf-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2adcf-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2adcf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2adcf-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2adcf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2adcf-122">Request headers</span></span>
|<span data-ttu-id="2adcf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2adcf-123">Header</span></span>|<span data-ttu-id="2adcf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2adcf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2adcf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2adcf-125">Authorization</span></span>|<span data-ttu-id="2adcf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2adcf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2adcf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2adcf-127">Accept</span></span>|<span data-ttu-id="2adcf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2adcf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2adcf-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2adcf-129">Request body</span></span>
<span data-ttu-id="2adcf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2adcf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2adcf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2adcf-131">Response</span></span>
<span data-ttu-id="2adcf-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2adcf-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2adcf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2adcf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2adcf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2adcf-134">Request</span></span>
<span data-ttu-id="2adcf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2adcf-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2adcf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2adcf-136">Response</span></span>
<span data-ttu-id="2adcf-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2adcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







