---
title: Удаление объекта enrollmentConfigurationAssignment
description: Удаляет объект enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3b274ad2d90d9dc7c8f663a3a93e3233072e5fb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709217"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="0ee00-103">Удаление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0ee00-103">Delete enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="0ee00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ee00-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee00-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ee00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee00-107">Удаляет объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0ee00-107">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee00-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ee00-108">Prerequisites</span></span>
<span data-ttu-id="0ee00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee00-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee00-111">Permission type</span></span>|<span data-ttu-id="0ee00-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ee00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee00-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ee00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee00-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee00-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee00-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ee00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee00-116">Not supported.</span></span>|
|<span data-ttu-id="0ee00-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ee00-117">Application</span></span>|<span data-ttu-id="0ee00-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee00-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee00-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ee00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0ee00-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ee00-120">Request headers</span></span>
|<span data-ttu-id="0ee00-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ee00-121">Header</span></span>|<span data-ttu-id="0ee00-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ee00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee00-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ee00-123">Authorization</span></span>|<span data-ttu-id="0ee00-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ee00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee00-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ee00-125">Accept</span></span>|<span data-ttu-id="0ee00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee00-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ee00-127">Request body</span></span>
<span data-ttu-id="0ee00-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ee00-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee00-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee00-129">Response</span></span>
<span data-ttu-id="0ee00-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ee00-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ee00-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ee00-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee00-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ee00-132">Request</span></span>
<span data-ttu-id="0ee00-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ee00-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0ee00-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee00-134">Response</span></span>
<span data-ttu-id="0ee00-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ee00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





