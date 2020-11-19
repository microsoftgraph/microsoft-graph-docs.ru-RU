---
title: Удаление Девицеманажементдериведкредентиалсеттингс
description: Удаляет объект Девицеманажементдериведкредентиалсеттингс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9721c92c82198a1ecb3996bb45acdaefcd948046
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210125"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="c0c5e-103">Удаление Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="c0c5e-103">Delete deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="c0c5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0c5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0c5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c5e-107">Удаляет объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c0c5e-107">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0c5e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0c5e-108">Prerequisites</span></span>
<span data-ttu-id="c0c5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c5e-111">Permission type</span></span>|<span data-ttu-id="c0c5e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0c5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0c5e-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c0c5e-114">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="c0c5e-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="c0c5e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c5e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c0c5e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0c5e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0c5e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-117">Not supported.</span></span>|
|<span data-ttu-id="c0c5e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0c5e-118">Application</span></span>||
|<span data-ttu-id="c0c5e-119">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="c0c5e-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="c0c5e-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c5e-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c5e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0c5e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="c0c5e-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0c5e-122">Request headers</span></span>
|<span data-ttu-id="c0c5e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0c5e-123">Header</span></span>|<span data-ttu-id="c0c5e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c0c5e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0c5e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0c5e-125">Authorization</span></span>|<span data-ttu-id="c0c5e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0c5e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c0c5e-127">Accept</span></span>|<span data-ttu-id="c0c5e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c5e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c5e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0c5e-129">Request body</span></span>
<span data-ttu-id="c0c5e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c5e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c5e-131">Response</span></span>
<span data-ttu-id="c0c5e-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0c5e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c0c5e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0c5e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0c5e-134">Request</span></span>
<span data-ttu-id="c0c5e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="c0c5e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c5e-136">Response</span></span>
<span data-ttu-id="c0c5e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0c5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








