---
title: Удаление windows10PkcsCertificateProfile
description: Удаляет windows10PkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: da86d71c3d04d58b8304f8c93bb15e257db1a82c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955915"
---
# <a name="delete-windows10pkcscertificateprofile"></a><span data-ttu-id="e4995-103">Удаление windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e4995-103">Delete windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="e4995-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4995-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4995-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4995-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4995-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e4995-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4995-107">Удаляет [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e4995-107">Deletes a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4995-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4995-108">Prerequisites</span></span>
<span data-ttu-id="e4995-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4995-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4995-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4995-111">Permission type</span></span>|<span data-ttu-id="e4995-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4995-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4995-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4995-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4995-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4995-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4995-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4995-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4995-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4995-116">Not supported.</span></span>|
|<span data-ttu-id="e4995-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4995-117">Application</span></span>|<span data-ttu-id="e4995-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4995-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4995-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4995-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e4995-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4995-120">Request headers</span></span>
|<span data-ttu-id="e4995-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4995-121">Header</span></span>|<span data-ttu-id="e4995-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4995-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4995-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4995-123">Authorization</span></span>|<span data-ttu-id="e4995-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e4995-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4995-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4995-125">Accept</span></span>|<span data-ttu-id="e4995-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4995-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4995-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4995-127">Request body</span></span>
<span data-ttu-id="e4995-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4995-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4995-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4995-129">Response</span></span>
<span data-ttu-id="e4995-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4995-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4995-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e4995-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4995-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4995-132">Request</span></span>
<span data-ttu-id="e4995-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4995-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e4995-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4995-134">Response</span></span>
<span data-ttu-id="e4995-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e4995-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





