---
title: Delete termsAndConditions
description: Удаляет объект termsAndConditions.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2a9b653d0b573f4d6adc275b5459163314c76ef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760174"
---
# <a name="delete-termsandconditions"></a><span data-ttu-id="fdd42-103">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="fdd42-103">Delete termsAndConditions</span></span>

> <span data-ttu-id="fdd42-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdd42-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdd42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdd42-106">Удаляет объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="fdd42-106">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdd42-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd42-107">Prerequisites</span></span>
<span data-ttu-id="fdd42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdd42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdd42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd42-110">Permission type</span></span>|<span data-ttu-id="fdd42-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdd42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdd42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdd42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdd42-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd42-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fdd42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdd42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdd42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd42-115">Not supported.</span></span>|
|<span data-ttu-id="fdd42-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fdd42-116">Application</span></span>|<span data-ttu-id="fdd42-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd42-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdd42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdd42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="fdd42-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fdd42-119">Request headers</span></span>
|<span data-ttu-id="fdd42-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdd42-120">Header</span></span>|<span data-ttu-id="fdd42-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fdd42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdd42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdd42-122">Authorization</span></span>|<span data-ttu-id="fdd42-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdd42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdd42-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fdd42-124">Accept</span></span>|<span data-ttu-id="fdd42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fdd42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdd42-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdd42-126">Request body</span></span>
<span data-ttu-id="fdd42-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdd42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdd42-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdd42-128">Response</span></span>
<span data-ttu-id="fdd42-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fdd42-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fdd42-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fdd42-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdd42-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdd42-131">Request</span></span>
<span data-ttu-id="fdd42-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdd42-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="fdd42-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdd42-133">Response</span></span>
<span data-ttu-id="fdd42-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdd42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




