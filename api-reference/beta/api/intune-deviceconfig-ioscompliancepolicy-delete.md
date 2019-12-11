---
title: Delete iosCompliancePolicy
description: Удаляет объект iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee8a72be8b76a43a83cbd064fde3f57e5cad8ad4
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949169"
---
# <a name="delete-ioscompliancepolicy"></a><span data-ttu-id="ef568-103">Delete iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ef568-103">Delete iosCompliancePolicy</span></span>

> <span data-ttu-id="ef568-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef568-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef568-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef568-106">Удаляет объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef568-106">Deletes a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef568-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ef568-107">Prerequisites</span></span>
<span data-ttu-id="ef568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef568-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef568-110">Permission type</span></span>|<span data-ttu-id="ef568-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef568-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef568-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef568-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef568-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef568-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef568-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef568-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef568-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef568-115">Not supported.</span></span>|
|<span data-ttu-id="ef568-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef568-116">Application</span></span>|<span data-ttu-id="ef568-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef568-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef568-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef568-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ef568-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef568-119">Request headers</span></span>
|<span data-ttu-id="ef568-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef568-120">Header</span></span>|<span data-ttu-id="ef568-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef568-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef568-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef568-122">Authorization</span></span>|<span data-ttu-id="ef568-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef568-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef568-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ef568-124">Accept</span></span>|<span data-ttu-id="ef568-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef568-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef568-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef568-126">Request body</span></span>
<span data-ttu-id="ef568-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef568-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef568-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef568-128">Response</span></span>
<span data-ttu-id="ef568-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef568-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef568-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ef568-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef568-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef568-131">Request</span></span>
<span data-ttu-id="ef568-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef568-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ef568-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef568-133">Response</span></span>
<span data-ttu-id="ef568-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef568-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





