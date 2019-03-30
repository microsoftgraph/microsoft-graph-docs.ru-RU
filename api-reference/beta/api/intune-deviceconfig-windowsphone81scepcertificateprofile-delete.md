---
title: Удаление windowsPhone81SCEPCertificateProfile
description: Удаляет объект windowsPhone81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fac195e2fd3b444bb3009475411ce26960069673
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986854"
---
# <a name="delete-windowsphone81scepcertificateprofile"></a><span data-ttu-id="a86ac-103">Удаление windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a86ac-103">Delete windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="a86ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a86ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a86ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a86ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a86ac-106">Удаляет объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a86ac-106">Deletes a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a86ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a86ac-107">Prerequisites</span></span>
<span data-ttu-id="a86ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a86ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a86ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a86ac-110">Permission type</span></span>|<span data-ttu-id="a86ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a86ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a86ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a86ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a86ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a86ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a86ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a86ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a86ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a86ac-115">Not supported.</span></span>|
|<span data-ttu-id="a86ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a86ac-116">Application</span></span>|<span data-ttu-id="a86ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a86ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a86ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a86ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a86ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a86ac-119">Request headers</span></span>
|<span data-ttu-id="a86ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a86ac-120">Header</span></span>|<span data-ttu-id="a86ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a86ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a86ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a86ac-122">Authorization</span></span>|<span data-ttu-id="a86ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a86ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a86ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a86ac-124">Accept</span></span>|<span data-ttu-id="a86ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a86ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a86ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a86ac-126">Request body</span></span>
<span data-ttu-id="a86ac-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a86ac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a86ac-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a86ac-128">Response</span></span>
<span data-ttu-id="a86ac-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a86ac-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a86ac-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a86ac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a86ac-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a86ac-131">Request</span></span>
<span data-ttu-id="a86ac-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a86ac-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a86ac-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a86ac-133">Response</span></span>
<span data-ttu-id="a86ac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a86ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




