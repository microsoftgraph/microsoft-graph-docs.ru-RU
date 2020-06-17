---
title: Удаление Комплианцеманажементпартнер
description: Удаляет объект Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d2c9cdc6571339ca38bf4f575d658de1c9cf83c
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744175"
---
# <a name="delete-compliancemanagementpartner"></a><span data-ttu-id="dbe6e-103">Удаление Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="dbe6e-103">Delete complianceManagementPartner</span></span>

<span data-ttu-id="dbe6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbe6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbe6e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbe6e-106">Удаляет объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="dbe6e-106">Deletes a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbe6e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dbe6e-107">Prerequisites</span></span>
<span data-ttu-id="dbe6e-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dbe6e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe6e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbe6e-110">Permission type</span></span>|<span data-ttu-id="dbe6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbe6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbe6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbe6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbe6e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe6e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dbe6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbe6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbe6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-115">Not supported.</span></span>|
|<span data-ttu-id="dbe6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbe6e-116">Application</span></span>|<span data-ttu-id="dbe6e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe6e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbe6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbe6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="dbe6e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dbe6e-119">Request headers</span></span>
|<span data-ttu-id="dbe6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbe6e-120">Header</span></span>|<span data-ttu-id="dbe6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dbe6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbe6e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbe6e-122">Authorization</span></span>|<span data-ttu-id="dbe6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbe6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dbe6e-124">Accept</span></span>|<span data-ttu-id="dbe6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbe6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbe6e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbe6e-126">Request body</span></span>
<span data-ttu-id="dbe6e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbe6e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbe6e-128">Response</span></span>
<span data-ttu-id="dbe6e-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dbe6e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dbe6e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbe6e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbe6e-131">Request</span></span>
<span data-ttu-id="dbe6e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="dbe6e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbe6e-133">Response</span></span>
<span data-ttu-id="dbe6e-134">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-134">Here is an example of the response.</span></span> <span data-ttu-id="dbe6e-135">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dbe6e-136">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dbe6e-136">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



