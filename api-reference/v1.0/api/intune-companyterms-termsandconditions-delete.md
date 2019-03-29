---
title: Delete termsAndConditions
description: Удаляет объект termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0169d4550884b72443429d558b865bbd0e998e4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982093"
---
# <a name="delete-termsandconditions"></a><span data-ttu-id="bb0ec-103">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bb0ec-103">Delete termsAndConditions</span></span>

> <span data-ttu-id="bb0ec-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0ec-105">Удаляет объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="bb0ec-105">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb0ec-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bb0ec-106">Prerequisites</span></span>
<span data-ttu-id="bb0ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb0ec-109">Permission type</span></span>|<span data-ttu-id="bb0ec-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb0ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb0ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb0ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb0ec-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb0ec-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bb0ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb0ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb0ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-114">Not supported.</span></span>|
|<span data-ttu-id="bb0ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb0ec-115">Application</span></span>|<span data-ttu-id="bb0ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb0ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb0ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="bb0ec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb0ec-118">Request headers</span></span>
|<span data-ttu-id="bb0ec-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb0ec-119">Header</span></span>|<span data-ttu-id="bb0ec-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bb0ec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb0ec-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb0ec-121">Authorization</span></span>|<span data-ttu-id="bb0ec-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb0ec-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb0ec-123">Accept</span></span>|<span data-ttu-id="bb0ec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb0ec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb0ec-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb0ec-125">Request body</span></span>
<span data-ttu-id="bb0ec-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb0ec-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb0ec-127">Response</span></span>
<span data-ttu-id="bb0ec-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb0ec-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bb0ec-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb0ec-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb0ec-130">Request</span></span>
<span data-ttu-id="bb0ec-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="bb0ec-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb0ec-132">Response</span></span>
<span data-ttu-id="bb0ec-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb0ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



