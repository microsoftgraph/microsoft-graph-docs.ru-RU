---
title: Удаление Девицеманажементдериведкредентиалсеттингс
description: Удаляет объект Девицеманажементдериведкредентиалсеттингс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cdc20d095fa50820c67548be47e7647e68cf76f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706312"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="e242b-103">Удаление Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="e242b-103">Delete deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="e242b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e242b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e242b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e242b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e242b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e242b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e242b-107">Удаляет объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="e242b-107">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e242b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e242b-108">Prerequisites</span></span>
<span data-ttu-id="e242b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e242b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e242b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e242b-111">Permission type</span></span>|<span data-ttu-id="e242b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e242b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e242b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e242b-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="e242b-114">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="e242b-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="e242b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e242b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e242b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e242b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e242b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e242b-117">Not supported.</span></span>|
|<span data-ttu-id="e242b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e242b-118">Application</span></span>||
|<span data-ttu-id="e242b-119">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="e242b-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="e242b-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e242b-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e242b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e242b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="e242b-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e242b-122">Request headers</span></span>
|<span data-ttu-id="e242b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e242b-123">Header</span></span>|<span data-ttu-id="e242b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e242b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e242b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e242b-125">Authorization</span></span>|<span data-ttu-id="e242b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e242b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e242b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e242b-127">Accept</span></span>|<span data-ttu-id="e242b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e242b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e242b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e242b-129">Request body</span></span>
<span data-ttu-id="e242b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e242b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e242b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e242b-131">Response</span></span>
<span data-ttu-id="e242b-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e242b-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e242b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e242b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e242b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e242b-134">Request</span></span>
<span data-ttu-id="e242b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e242b-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="e242b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e242b-136">Response</span></span>
<span data-ttu-id="e242b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e242b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









