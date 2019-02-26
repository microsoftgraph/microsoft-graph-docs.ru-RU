---
title: Удаление объекта enrollmentConfigurationAssignment
description: Удаляет объект enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f737e3a2c4a407c0ad9731ef9dcda006ae295f8a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258291"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="1c260-103">Удаление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c260-103">Delete enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="1c260-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c260-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c260-105">Удаляет объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c260-105">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c260-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c260-106">Prerequisites</span></span>
<span data-ttu-id="1c260-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c260-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c260-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c260-109">Permission type</span></span>|<span data-ttu-id="1c260-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c260-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c260-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c260-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c260-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c260-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1c260-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c260-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c260-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c260-114">Not supported.</span></span>|
|<span data-ttu-id="1c260-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c260-115">Application</span></span>|<span data-ttu-id="1c260-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c260-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c260-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c260-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1c260-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c260-118">Request headers</span></span>
|<span data-ttu-id="1c260-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c260-119">Header</span></span>|<span data-ttu-id="1c260-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1c260-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c260-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c260-121">Authorization</span></span>|<span data-ttu-id="1c260-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1c260-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c260-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1c260-123">Accept</span></span>|<span data-ttu-id="1c260-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c260-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c260-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c260-125">Request body</span></span>
<span data-ttu-id="1c260-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c260-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c260-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c260-127">Response</span></span>
<span data-ttu-id="1c260-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c260-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c260-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1c260-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c260-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c260-130">Request</span></span>
<span data-ttu-id="1c260-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c260-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="1c260-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="1c260-132">Response</span></span>
<span data-ttu-id="1c260-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c260-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



