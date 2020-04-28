---
title: Delete termsAndConditions
description: Удаляет объект termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c60b4864f5355fdda14a0a124388f1a85013e63c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436604"
---
# <a name="delete-termsandconditions"></a><span data-ttu-id="c3e36-103">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="c3e36-103">Delete termsAndConditions</span></span>

<span data-ttu-id="c3e36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3e36-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3e36-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3e36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3e36-107">Удаляет объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="c3e36-107">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3e36-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e36-108">Prerequisites</span></span>
<span data-ttu-id="c3e36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3e36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e36-111">Permission type</span></span>|<span data-ttu-id="c3e36-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3e36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3e36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3e36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3e36-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e36-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3e36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3e36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3e36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e36-116">Not supported.</span></span>|
|<span data-ttu-id="c3e36-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3e36-117">Application</span></span>|<span data-ttu-id="c3e36-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e36-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3e36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="c3e36-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3e36-120">Request headers</span></span>
|<span data-ttu-id="c3e36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3e36-121">Header</span></span>|<span data-ttu-id="c3e36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3e36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3e36-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3e36-123">Authorization</span></span>|<span data-ttu-id="c3e36-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3e36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3e36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3e36-125">Accept</span></span>|<span data-ttu-id="c3e36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3e36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3e36-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3e36-127">Request body</span></span>
<span data-ttu-id="c3e36-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3e36-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3e36-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3e36-129">Response</span></span>
<span data-ttu-id="c3e36-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3e36-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c3e36-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3e36-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3e36-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3e36-132">Request</span></span>
<span data-ttu-id="c3e36-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3e36-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="c3e36-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3e36-134">Response</span></span>
<span data-ttu-id="c3e36-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3e36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



