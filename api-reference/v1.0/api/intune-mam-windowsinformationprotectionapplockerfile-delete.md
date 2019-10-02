---
title: Удаление объекта windowsInformationProtectionAppLockerFile
description: Удаляет объект windowsInformationProtectionAppLockerFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 169e65d68a96dedb5abd41ab7d82f95625df9e34
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363054"
---
# <a name="delete-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="4c330-103">Удаление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="4c330-103">Delete windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="4c330-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c330-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c330-105">Удаляет объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="4c330-105">Deletes a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c330-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c330-106">Prerequisites</span></span>
<span data-ttu-id="4c330-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c330-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c330-109">Permission type</span></span>|<span data-ttu-id="4c330-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c330-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c330-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c330-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c330-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c330-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c330-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c330-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c330-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c330-114">Not supported.</span></span>|
|<span data-ttu-id="4c330-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c330-115">Application</span></span>|<span data-ttu-id="4c330-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c330-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c330-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c330-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="4c330-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c330-118">Request headers</span></span>
|<span data-ttu-id="4c330-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c330-119">Header</span></span>|<span data-ttu-id="4c330-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4c330-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c330-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c330-121">Authorization</span></span>|<span data-ttu-id="4c330-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c330-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c330-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4c330-123">Accept</span></span>|<span data-ttu-id="4c330-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c330-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c330-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c330-125">Request body</span></span>
<span data-ttu-id="4c330-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c330-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c330-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c330-127">Response</span></span>
<span data-ttu-id="4c330-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c330-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c330-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4c330-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c330-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c330-130">Request</span></span>
<span data-ttu-id="4c330-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c330-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="4c330-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c330-132">Response</span></span>
<span data-ttu-id="4c330-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c330-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




