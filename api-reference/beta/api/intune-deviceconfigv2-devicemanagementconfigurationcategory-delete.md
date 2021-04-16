---
title: Удаление deviceManagementConfigurationCategory
description: Удаляет устройствоManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30ad012f94bc81d80488005623dc62c03aedfe5f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866281"
---
# <a name="delete-devicemanagementconfigurationcategory"></a><span data-ttu-id="2235f-103">Удаление deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="2235f-103">Delete deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="2235f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2235f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2235f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2235f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2235f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2235f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2235f-107">Удаляет [устройствоManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="2235f-107">Deletes a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2235f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2235f-108">Prerequisites</span></span>
<span data-ttu-id="2235f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2235f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2235f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2235f-111">Permission type</span></span>|<span data-ttu-id="2235f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2235f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2235f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2235f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2235f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2235f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2235f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2235f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2235f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2235f-116">Not supported.</span></span>|
|<span data-ttu-id="2235f-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2235f-117">Application</span></span>|<span data-ttu-id="2235f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2235f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2235f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2235f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="2235f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2235f-120">Request headers</span></span>
|<span data-ttu-id="2235f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2235f-121">Header</span></span>|<span data-ttu-id="2235f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2235f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2235f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2235f-123">Authorization</span></span>|<span data-ttu-id="2235f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2235f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2235f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2235f-125">Accept</span></span>|<span data-ttu-id="2235f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2235f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2235f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2235f-127">Request body</span></span>
<span data-ttu-id="2235f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2235f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2235f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2235f-129">Response</span></span>
<span data-ttu-id="2235f-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2235f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2235f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2235f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2235f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2235f-132">Request</span></span>
<span data-ttu-id="2235f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2235f-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

### <a name="response"></a><span data-ttu-id="2235f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2235f-134">Response</span></span>
<span data-ttu-id="2235f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2235f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




