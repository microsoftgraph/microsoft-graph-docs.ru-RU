---
title: Delete termsAndConditionsAcceptanceStatus
description: Удаляет объект termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4043a71ee87ccadc8e829c045dc0c1fe0f77d23c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933867"
---
# <a name="delete-termsandconditionsacceptancestatus"></a><span data-ttu-id="1d805-103">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1d805-103">Delete termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="1d805-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d805-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d805-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d805-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d805-106">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1d805-106">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d805-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1d805-107">Prerequisites</span></span>
<span data-ttu-id="1d805-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d805-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d805-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d805-110">Permission type</span></span>|<span data-ttu-id="1d805-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d805-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d805-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d805-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d805-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d805-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d805-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d805-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d805-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d805-115">Not supported.</span></span>|
|<span data-ttu-id="1d805-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d805-116">Application</span></span>|<span data-ttu-id="1d805-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d805-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d805-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d805-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1d805-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d805-119">Request headers</span></span>
|<span data-ttu-id="1d805-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d805-120">Header</span></span>|<span data-ttu-id="1d805-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1d805-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d805-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d805-122">Authorization</span></span>|<span data-ttu-id="1d805-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d805-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d805-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1d805-124">Accept</span></span>|<span data-ttu-id="1d805-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d805-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d805-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d805-126">Request body</span></span>
<span data-ttu-id="1d805-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d805-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d805-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d805-128">Response</span></span>
<span data-ttu-id="1d805-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1d805-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1d805-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1d805-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d805-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d805-131">Request</span></span>
<span data-ttu-id="1d805-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d805-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="1d805-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d805-133">Response</span></span>
<span data-ttu-id="1d805-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d805-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




