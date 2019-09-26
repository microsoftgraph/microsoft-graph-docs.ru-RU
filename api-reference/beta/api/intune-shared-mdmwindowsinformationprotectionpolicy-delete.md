---
title: Удаление объекта mdmWindowsInformationProtectionPolicy
description: Удаляет объект mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e44aa4e173d7de3b1d3f5fa9f70cd297fdc9e52
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201168"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="5bae3-103">Удаление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5bae3-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="5bae3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bae3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bae3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bae3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bae3-106">Удаляет объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5bae3-106">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bae3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5bae3-107">Prerequisites</span></span>
<span data-ttu-id="5bae3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bae3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bae3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bae3-110">Permission type</span></span>|<span data-ttu-id="5bae3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bae3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bae3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bae3-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5bae3-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="5bae3-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="5bae3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bae3-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="5bae3-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5bae3-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5bae3-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bae3-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bae3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bae3-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bae3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bae3-118">Not supported.</span></span>|
|<span data-ttu-id="5bae3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bae3-119">Application</span></span>||
| <span data-ttu-id="5bae3-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="5bae3-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="5bae3-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bae3-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="5bae3-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5bae3-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5bae3-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bae3-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bae3-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bae3-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5bae3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bae3-125">Request headers</span></span>
|<span data-ttu-id="5bae3-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bae3-126">Header</span></span>|<span data-ttu-id="5bae3-127">Значение</span><span class="sxs-lookup"><span data-stu-id="5bae3-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bae3-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bae3-128">Authorization</span></span>|<span data-ttu-id="5bae3-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bae3-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bae3-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5bae3-130">Accept</span></span>|<span data-ttu-id="5bae3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5bae3-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bae3-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bae3-132">Request body</span></span>
<span data-ttu-id="5bae3-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bae3-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bae3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bae3-134">Response</span></span>
<span data-ttu-id="5bae3-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5bae3-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5bae3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5bae3-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bae3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bae3-137">Request</span></span>
<span data-ttu-id="5bae3-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bae3-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="5bae3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bae3-139">Response</span></span>
<span data-ttu-id="5bae3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bae3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




