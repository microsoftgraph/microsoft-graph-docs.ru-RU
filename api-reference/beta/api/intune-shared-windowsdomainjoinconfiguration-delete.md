---
title: Удаление Виндовсдомаинжоинконфигуратион
description: Удаляет объект Виндовсдомаинжоинконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74cc1c53712bd20406209fc7ceca47d5eceb5786
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526813"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="d15b8-103">Удаление Виндовсдомаинжоинконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d15b8-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="d15b8-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d15b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d15b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d15b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d15b8-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d15b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d15b8-107">Удаляет объект [виндовсдомаинжоинконфигуратион](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d15b8-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d15b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d15b8-108">Prerequisites</span></span>
<span data-ttu-id="d15b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d15b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d15b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d15b8-111">Permission type</span></span>|<span data-ttu-id="d15b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d15b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d15b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d15b8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d15b8-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="d15b8-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d15b8-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15b8-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="d15b8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d15b8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d15b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d15b8-117">Not supported.</span></span>|
|<span data-ttu-id="d15b8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d15b8-118">Application</span></span>|<span data-ttu-id="d15b8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d15b8-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d15b8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d15b8-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d15b8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d15b8-121">Request headers</span></span>
|<span data-ttu-id="d15b8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d15b8-122">Header</span></span>|<span data-ttu-id="d15b8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d15b8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d15b8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d15b8-124">Authorization</span></span>|<span data-ttu-id="d15b8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d15b8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d15b8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d15b8-126">Accept</span></span>|<span data-ttu-id="d15b8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d15b8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d15b8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d15b8-128">Request body</span></span>
<span data-ttu-id="d15b8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d15b8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d15b8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d15b8-130">Response</span></span>
<span data-ttu-id="d15b8-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d15b8-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d15b8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d15b8-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="d15b8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d15b8-133">Request</span></span>
<span data-ttu-id="d15b8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d15b8-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d15b8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d15b8-135">Response</span></span>
<span data-ttu-id="d15b8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d15b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



