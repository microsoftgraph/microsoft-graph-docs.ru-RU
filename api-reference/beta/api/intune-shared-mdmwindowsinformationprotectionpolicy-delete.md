---
title: Удаление объекта mdmWindowsInformationProtectionPolicy
description: Удаляет объект mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7268b7754629fb87a6f32acac84c005dfb513c98
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863046"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="a623e-103">Удаление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a623e-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="a623e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a623e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a623e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a623e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a623e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a623e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a623e-107">Удаляет объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a623e-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a623e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a623e-108">Prerequisites</span></span>
<span data-ttu-id="a623e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a623e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a623e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a623e-111">Permission type</span></span>|<span data-ttu-id="a623e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a623e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a623e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a623e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a623e-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a623e-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="a623e-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a623e-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="a623e-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a623e-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a623e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a623e-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a623e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a623e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a623e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a623e-119">Not supported.</span></span>|
|<span data-ttu-id="a623e-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a623e-120">Application</span></span>||
| <span data-ttu-id="a623e-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a623e-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="a623e-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a623e-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="a623e-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a623e-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a623e-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a623e-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a623e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a623e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a623e-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a623e-126">Request headers</span></span>
|<span data-ttu-id="a623e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a623e-127">Header</span></span>|<span data-ttu-id="a623e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a623e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a623e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a623e-129">Authorization</span></span>|<span data-ttu-id="a623e-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a623e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a623e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="a623e-131">Accept</span></span>|<span data-ttu-id="a623e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="a623e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a623e-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a623e-133">Request body</span></span>
<span data-ttu-id="a623e-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a623e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a623e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a623e-135">Response</span></span>
<span data-ttu-id="a623e-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a623e-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a623e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a623e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a623e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a623e-138">Request</span></span>
<span data-ttu-id="a623e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a623e-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="a623e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a623e-140">Response</span></span>
<span data-ttu-id="a623e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a623e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







