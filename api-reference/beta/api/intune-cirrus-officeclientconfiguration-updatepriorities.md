---
title: Действие updatePriorities
description: Обновление приоритетов политики.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc2ddb07589729db0a51aee885133ad2474965d0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760293"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="3eb57-103">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="3eb57-103">updatePriorities action</span></span>

> <span data-ttu-id="3eb57-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eb57-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3eb57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb57-106">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="3eb57-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eb57-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3eb57-107">Prerequisites</span></span>
<span data-ttu-id="3eb57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb57-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eb57-110">Permission type</span></span>|<span data-ttu-id="3eb57-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eb57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb57-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eb57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb57-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb57-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb57-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eb57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb57-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb57-115">Not supported.</span></span>|
|<span data-ttu-id="3eb57-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3eb57-116">Application</span></span>|<span data-ttu-id="3eb57-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb57-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb57-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eb57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="3eb57-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3eb57-119">Request headers</span></span>
|<span data-ttu-id="3eb57-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3eb57-120">Header</span></span>|<span data-ttu-id="3eb57-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3eb57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb57-122">Authorization</span></span>|<span data-ttu-id="3eb57-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eb57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb57-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3eb57-124">Accept</span></span>|<span data-ttu-id="3eb57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb57-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eb57-126">Request body</span></span>
<span data-ttu-id="3eb57-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eb57-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3eb57-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3eb57-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3eb57-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eb57-129">Property</span></span>|<span data-ttu-id="3eb57-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3eb57-130">Type</span></span>|<span data-ttu-id="3eb57-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3eb57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb57-132">оффицеконфигуратионполициидс</span><span class="sxs-lookup"><span data-stu-id="3eb57-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="3eb57-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3eb57-133">String collection</span></span>|<span data-ttu-id="3eb57-134">Список идентификаторов политик конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="3eb57-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="3eb57-135">оффицеконфигуратионприоритиес</span><span class="sxs-lookup"><span data-stu-id="3eb57-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="3eb57-136">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="3eb57-136">Int32 collection</span></span>|<span data-ttu-id="3eb57-137">Список приоритетов конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="3eb57-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="3eb57-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="3eb57-138">Response</span></span>
<span data-ttu-id="3eb57-139">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3eb57-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3eb57-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3eb57-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eb57-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eb57-141">Request</span></span>
<span data-ttu-id="3eb57-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eb57-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities

Content-type: application/json
Content-length: 143

{
  "officeConfigurationPolicyIds": [
    "Office Configuration Policy Ids value"
  ],
  "officeConfigurationPriorities": [
    13
  ]
}
```

### <a name="response"></a><span data-ttu-id="3eb57-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb57-143">Response</span></span>
<span data-ttu-id="3eb57-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3eb57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




