---
title: Удаление Комплианцеманажементпартнер
description: Удаляет объект Комплианцеманажементпартнер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8683c82ee203a16c822a288a171d32d717191a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462524"
---
# <a name="delete-compliancemanagementpartner"></a><span data-ttu-id="df1eb-103">Удаление Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="df1eb-103">Delete complianceManagementPartner</span></span>

<span data-ttu-id="df1eb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="df1eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df1eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df1eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df1eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df1eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df1eb-107">Удаляет объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="df1eb-107">Deletes a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df1eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="df1eb-108">Prerequisites</span></span>
<span data-ttu-id="df1eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df1eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df1eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df1eb-111">Permission type</span></span>|<span data-ttu-id="df1eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df1eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df1eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df1eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df1eb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df1eb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df1eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df1eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df1eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df1eb-116">Not supported.</span></span>|
|<span data-ttu-id="df1eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df1eb-117">Application</span></span>|<span data-ttu-id="df1eb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df1eb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df1eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df1eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="df1eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df1eb-120">Request headers</span></span>
|<span data-ttu-id="df1eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df1eb-121">Header</span></span>|<span data-ttu-id="df1eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df1eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df1eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df1eb-123">Authorization</span></span>|<span data-ttu-id="df1eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df1eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df1eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df1eb-125">Accept</span></span>|<span data-ttu-id="df1eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df1eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df1eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df1eb-127">Request body</span></span>
<span data-ttu-id="df1eb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df1eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df1eb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="df1eb-129">Response</span></span>
<span data-ttu-id="df1eb-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df1eb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df1eb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="df1eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df1eb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="df1eb-132">Request</span></span>
<span data-ttu-id="df1eb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df1eb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="df1eb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="df1eb-134">Response</span></span>
<span data-ttu-id="df1eb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df1eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





