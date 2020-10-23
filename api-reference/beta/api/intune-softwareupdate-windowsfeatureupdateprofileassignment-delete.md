---
title: Удаление Виндовсфеатуреупдатепрофилеассигнмент
description: Удаляет объект Виндовсфеатуреупдатепрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c8aea2941b549cf04570886e55869938f3cb533
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695196"
---
# <a name="delete-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="1f2de-103">Удаление Виндовсфеатуреупдатепрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="1f2de-103">Delete windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="1f2de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f2de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f2de-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f2de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f2de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f2de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f2de-107">Удаляет объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1f2de-107">Deletes a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f2de-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f2de-108">Prerequisites</span></span>
<span data-ttu-id="1f2de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f2de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f2de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f2de-111">Permission type</span></span>|<span data-ttu-id="1f2de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f2de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f2de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f2de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f2de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f2de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f2de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f2de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f2de-116">Not supported.</span></span>|
|<span data-ttu-id="1f2de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f2de-117">Application</span></span>|<span data-ttu-id="1f2de-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2de-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f2de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f2de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1f2de-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f2de-120">Request headers</span></span>
|<span data-ttu-id="1f2de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f2de-121">Header</span></span>|<span data-ttu-id="1f2de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f2de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f2de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f2de-123">Authorization</span></span>|<span data-ttu-id="1f2de-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f2de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f2de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f2de-125">Accept</span></span>|<span data-ttu-id="1f2de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f2de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f2de-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f2de-127">Request body</span></span>
<span data-ttu-id="1f2de-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f2de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f2de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f2de-129">Response</span></span>
<span data-ttu-id="1f2de-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1f2de-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f2de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1f2de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f2de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f2de-132">Request</span></span>
<span data-ttu-id="1f2de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f2de-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="1f2de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f2de-134">Response</span></span>
<span data-ttu-id="1f2de-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f2de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





