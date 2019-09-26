---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cb29c5212d44c9affa895dc9dbe15b56e74e146
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201140"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="c3a84-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="c3a84-103">Delete windowsUpdateState</span></span>

> <span data-ttu-id="c3a84-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a84-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3a84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a84-106">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="c3a84-106">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3a84-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3a84-107">Prerequisites</span></span>
<span data-ttu-id="c3a84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3a84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a84-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3a84-110">Permission type</span></span>|<span data-ttu-id="c3a84-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3a84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3a84-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3a84-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c3a84-113">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="c3a84-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c3a84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c3a84-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c3a84-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c3a84-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a84-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3a84-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3a84-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3a84-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a84-118">Not supported.</span></span>|
|<span data-ttu-id="c3a84-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3a84-119">Application</span></span>||
| <span data-ttu-id="c3a84-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="c3a84-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c3a84-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a84-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c3a84-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c3a84-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c3a84-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a84-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3a84-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3a84-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c3a84-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3a84-125">Request headers</span></span>
|<span data-ttu-id="c3a84-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3a84-126">Header</span></span>|<span data-ttu-id="c3a84-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c3a84-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3a84-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3a84-128">Authorization</span></span>|<span data-ttu-id="c3a84-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3a84-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3a84-130">Accept</span><span class="sxs-lookup"><span data-stu-id="c3a84-130">Accept</span></span>|<span data-ttu-id="c3a84-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c3a84-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3a84-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3a84-132">Request body</span></span>
<span data-ttu-id="c3a84-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3a84-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3a84-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a84-134">Response</span></span>
<span data-ttu-id="c3a84-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3a84-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c3a84-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a84-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3a84-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a84-137">Request</span></span>
<span data-ttu-id="c3a84-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3a84-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="c3a84-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a84-139">Response</span></span>
<span data-ttu-id="c3a84-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3a84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




