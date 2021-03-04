---
title: Удаление userExperienceAnalyticsRemoteConnection
description: Удаляет пользователяExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4db3e45960f9fe56e5fd370e169548755c42a52f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447434"
---
# <a name="delete-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="f6b87-103">Удаление userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="f6b87-103">Delete userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="f6b87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6b87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6b87-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6b87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6b87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6b87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6b87-107">Удаляет [пользователяExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f6b87-107">Deletes a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6b87-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6b87-108">Prerequisites</span></span>
<span data-ttu-id="f6b87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6b87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6b87-111">Permission type</span></span>|<span data-ttu-id="f6b87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6b87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6b87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6b87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6b87-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6b87-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f6b87-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6b87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6b87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6b87-116">Not supported.</span></span>|
|<span data-ttu-id="f6b87-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6b87-117">Application</span></span>|<span data-ttu-id="f6b87-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6b87-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6b87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6b87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="request-headers"></a><span data-ttu-id="f6b87-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6b87-120">Request headers</span></span>
|<span data-ttu-id="f6b87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6b87-121">Header</span></span>|<span data-ttu-id="f6b87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6b87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6b87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6b87-123">Authorization</span></span>|<span data-ttu-id="f6b87-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6b87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6b87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6b87-125">Accept</span></span>|<span data-ttu-id="f6b87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6b87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6b87-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6b87-127">Request body</span></span>
<span data-ttu-id="f6b87-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6b87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6b87-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6b87-129">Response</span></span>
<span data-ttu-id="f6b87-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6b87-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6b87-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f6b87-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6b87-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6b87-132">Request</span></span>
<span data-ttu-id="f6b87-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6b87-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

### <a name="response"></a><span data-ttu-id="f6b87-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6b87-134">Response</span></span>
<span data-ttu-id="f6b87-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6b87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




