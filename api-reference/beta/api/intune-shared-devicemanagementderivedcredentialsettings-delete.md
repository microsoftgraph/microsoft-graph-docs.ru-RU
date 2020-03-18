---
title: Удаление Девицеманажементдериведкредентиалсеттингс
description: Удаляет объект Девицеманажементдериведкредентиалсеттингс.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c0cfabb9571ad08458c628b0e8871fda90e35ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801021"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="24cea-103">Удаление Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="24cea-103">Delete deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="24cea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24cea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24cea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24cea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24cea-106">Удаляет объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="24cea-106">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24cea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24cea-107">Prerequisites</span></span>
<span data-ttu-id="24cea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24cea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24cea-110">Permission type</span></span>|<span data-ttu-id="24cea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24cea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24cea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24cea-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="24cea-113">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="24cea-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="24cea-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24cea-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24cea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24cea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24cea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24cea-116">Not supported.</span></span>|
|<span data-ttu-id="24cea-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24cea-117">Application</span></span>||
|<span data-ttu-id="24cea-118">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="24cea-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="24cea-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24cea-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24cea-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24cea-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="24cea-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24cea-121">Request headers</span></span>
|<span data-ttu-id="24cea-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24cea-122">Header</span></span>|<span data-ttu-id="24cea-123">Значение</span><span class="sxs-lookup"><span data-stu-id="24cea-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24cea-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="24cea-124">Authorization</span></span>|<span data-ttu-id="24cea-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24cea-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24cea-126">Accept</span><span class="sxs-lookup"><span data-stu-id="24cea-126">Accept</span></span>|<span data-ttu-id="24cea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24cea-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24cea-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24cea-128">Request body</span></span>
<span data-ttu-id="24cea-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24cea-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24cea-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="24cea-130">Response</span></span>
<span data-ttu-id="24cea-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24cea-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="24cea-132">Пример</span><span class="sxs-lookup"><span data-stu-id="24cea-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24cea-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="24cea-133">Request</span></span>
<span data-ttu-id="24cea-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24cea-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="24cea-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="24cea-135">Response</span></span>
<span data-ttu-id="24cea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24cea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








